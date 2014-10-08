require 'json'
require 'yaml'
require 'csv'

# ISO 3166-1			http://en.wikipedia.org/wiki/ISO_3166-1
# ISO 3166-1 alpha-2	http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2
# ISO 3166-1 alpha-3	http://en.wikipedia.org/wiki/ISO_3166-1_alpha-3
# ISO 3166-2 			http://en.wikipedia.org/wiki/ISO_3166-2
# http://www.millometro.com/ais/mmsi.pdf

data = {
	# 3166-1 alpha-2, 3166-1 alpha-3, 3166-2, Country Name
	201 =>	['AL', 'ALB', '', 		'Albania (Republic of)'],
	202	=>	['AD', 'AND', '', 		'Andorra (Principality of)'],
	203	=>	['AT', 'AUT', '', 		'Austria'],
	204	=>	['PT', 'PRT', 'PT-20', 	'Azores - Portugal'],
	205	=>	['BE', 'BEL', '', 		'Belgium'],
	206	=>	['BY', 'BLR', '', 		'Belarus (Republic of)'],
	207	=>	['BG', 'BGR', '', 		'Bulgaria (Republic of)'],
	208	=>	['VA', 'VAT', '',		'Vatican City State'],
	209	=>	['CY', 'CYP', '', 		'Cyprus (Republic of)'],
	210 =>	['CY', 'CYP', '', 		'Cyprus (Republic of)'],
	211	=>	['DE', 'DEU', '', 		'Germany (Federal Republic of)'],
	212	=>	['CY', 'CYP', '',		'Cyprus (Republic of)'],
	213	=>	['GE', 'GEO', '', 		'Georgia'],
	214	=>	['MD', 'MDA', '',		'Moldova (Republic of)'],
	215	=>	['MT', 'MLT', '',		'Malta'],
	216	=>	['AM', 'ARM', '',		'Armenia (Republic of)'],
	218	=>	['DE', 'DEU', '', 		'Germany (Federal Republic of)'],
	219 =>	['DK', 'DNK', '',		'Denmark'],
	220 =>	['DK', 'DNK', '',		'Denmark'],
	224 =>	['ES', 'ESP', '',		'Spain'],
	225 =>	['ES', 'ESP', '',		'Spain'],
	226 =>	['FR', 'FRA', '',		'France'],
	227 =>	['FR', 'FRA', '',		'France'],
	228 =>	['FR', 'FRA', '',		'France'],
	228 =>	['MT', 'MLT', '',		'Malta'],
	230 =>	['FI', 'FIN', '',		'Finland'],
	231 =>	['FO', 'FRO', '',		'Faroe Islands - Denmark'],
	232 =>	['GB', 'GBR', '',		'United Kingdom of Great Britain and Northern Ireland'],
	233 =>	['GB', 'GBR', '',		'United Kingdom of Great Britain and Northern Ireland'],
	234 =>	['GB', 'GBR', '',		'United Kingdom of Great Britain and Northern Ireland'],
	235 =>	['GB', 'GBR', '',		'United Kingdom of Great Britain and Northern Ireland'],
	236 =>	['GI', 'GIB', '',		'Gibraltar - United Kingdom of Great Britain and Northern Ireland'],
	237 =>	['GR', 'GRC', '',		'Greece'],
	238	=>	['HR', 'HRV', '',		'Croatia (Republic of)'],
	239 =>	['GR', 'GRC', '',		'Greece'],
	240 =>	['GR', 'GRC', '',		'Greece'],
	241 =>	['GR', 'GRC', '',		'Greece'],
	242	=>	['MA', 'MAR', '',		'Morocco (Kingdom of)'],
	243 =>	['HU', 'HUN', '',		'Hungary'],
	244 =>	['NL', 'NLD', '',		'Netherlands (Kingdom of the)'],
	245 =>	['NL', 'NLD', '',		'Netherlands (Kingdom of the)'],
	246 =>	['NL', 'NLD', '',		'Netherlands (Kingdom of the)'],
	247 =>	['IT', 'ITA', '',		'Italy'],
	248 =>	['MT', 'MLT', '',		'Malta'],
	250 =>	['IE', 'IRL', '',		'Ireland'],
	251 =>	['IS', 'ISL', '',		'Iceland'],
	252 =>	['LI', 'LIE', '',		'Liechtenstein (Principality of)'],
	253 =>	['LU', 'LUX', '',		'Luxembourg'],
	254 =>	['MC', 'MCO', '',		'Monaco (Principality of)'],
	255 =>	['PT', 'PRT', 'PT-30',	'Madeira - Portugal'],
	256 =>	['MT', 'MLT', '',		'Malta'],
	257 =>	['NO', 'NOR', '',		'Norway'],
	258 =>	['NO', 'NOR', '',		'Norway'],
	259 =>	['NO', 'NOR', '',		'Norway'],
	261 =>	['PL', 'POL', '',		'Poland (Republic of)'],
	262 =>	['ME', 'MNE', '',		'Montenegro'],
	263	=>	['PT', 'PRT', '', 		'Portugal'],
	264	=>	['RO', 'ROU', '', 		'Romania'],
	265	=>	['SE', 'SWE', '', 		'Sweden'],
	266	=>	['SE', 'SWE', '', 		'Sweden'],
	267	=>	['SK', 'SVK', '', 		'Slovak Republic'],
	268	=>	['SM', 'SMR', '', 		'San Marino (Republic of)'],
	269	=>	['CH', 'CHE', '', 		'Switzerland (Confederation of)'],
	270	=>	['CZ', 'CZE', '', 		'Czech Republic'],
	271	=>	['TR', 'TUR', '', 		'Turkey'],
	272	=>	['UA', 'UKR', '', 		'Ukraine'],
	273	=>	['RU', 'RUS', '',		'Russian Federation'],
 	274	=>	['MK', 'MKD', '',		'The Former Yugoslav Republic of Macedonia'],
 	275	=>	['LV', 'LVA', '', 		'Latvia (Republic of)'],
 	276 =>	['EE', 'EST', '',		'Estonia (Republic of)'],
 	277	=>	['LT', 'LTU', '',		'Lithuania (Republic of)'],
 	278	=>	['SI', 'SVN', '',		'Slovenia (Republic of)'],
 	279 =>	['RS', 'SRB', '',		'Serbia (Republic of)'],
 	301	=>	['AI', 'AIA', '',		'Anguilla - United Kingdom of Great Britain and Northern Ireland'],
 	303	=>	['US', 'USA', 'US-AK',	'Alaska (State of) - United States of America'],
 	304 =>	['AG', 'ATG', '', 		'Antigua and Barbuda'],
 	305	=>	['AG', 'ATG', '', 		'Antigua and Barbuda'],
 	306	=>	['CW', 'CUW', '', 		'Antilles - Netherlands (Kingdom of the)'],
	307	=>	['AW', 'ABW', '',		'Aruba - Netherlands (Kingdom of the)'],
	308	=>	['BS', 'BHS', '',		'Bahamas (Commonwealth of the)'],
	309	=>	['BS', 'BHS', '',		'Bahamas (Commonwealth of the)'],
	310	=>	['BM', 'BMU', '',		'Bermuda - United Kingdom of Great Britain and Northern Ireland'],
	311	=>	['BS', 'BMU', '',		'Bahamas (Commonwealth of the)'],
	312	=>	['BZ', 'BLZ', '',		'Belize'],
	314	=>	['BB', 'BRB', '',		'Barbados'],
	316	=>	['CA', 'CAN', '',		'Canada'],
	319	=>	['KY', 'CYM', '',		'Cayman Islands - United Kingdom of Great Britain and Northern Ireland'],
	321 =>	['CR', 'CRI', '',		'Costa Rica'],
	323 =>	['CU', 'CUB', '',		'Cuba'],
	325 =>	['DM', 'DMA', '',		'Dominica (Commonwealth of)'],
	327 =>	['DO', 'DOM', '',		'Dominican Republic'],
	329 =>	['GP', 'GLP', '',		'Guadeloupe (French Department of) - France'],
	330 =>	['GD', 'GRD', '',		'Grenada'],
	331	=>	['GL', 'GRL', '',		'Greenland - Denmark'],
	332	=>	['GT', 'GTM', '',		'Guatemala (Republic of)'],
	335 =>	['HN', 'HND', '',		'Honduras (Republic of)'],
	336	=>	['HT', 'HTI', '',		'Haiti (Republic of)'],
	338	=>	['US', 'USA', '',		'United States of America'],
	339	=>	['JM', 'JAM', '',		'Jamaica'],
	341	=>	['KN', 'KNA', '',		'Saint Kitts and Nevis (Federation of)'],
	343	=>	['LC', 'LCA', '',		'Saint Lucia'],
	345	=>	['MX', 'MEX', '',		'Mexico'],
	347	=>	['MQ', 'MTQ', '',		'Martinique (French Department of) - France'],
	348 =>	['MS', 'MSR', '',		'Montserrat - United Kingdom of Great Britain and Northern Ireland'],
	350 =>	['NI', 'NIC', '',		'Nicaragua'],
	351 =>	['PA', 'PAN', '',		'Panama (Republic of)'],
	352 =>	['PA', 'PAN', '',		'Panama (Republic of)'],
	353 =>	['PA', 'PAN', '',		'Panama (Republic of)'],
	354 =>	['PA', 'PAN', '',		'Panama (Republic of)'],
	# 355,356, 357	-
	358 =>	['PR', 'PRI', '',		'Puerto Rico - United States of America'],
	359 =>	['SV', 'SLV', '',		'El Salvador (Republic of)'],
	361 =>	['PM', 'SPM', '',		'Saint Pierre and Miquelon (Territorial Collectivity of) - France'],
	362	=>	['TT', 'TTO', '',		'Trinidad and Tobago'],
	364	=>	['TC', 'TCA', '',		'Turks and Caicos Islands - United Kingdom of Great Britain and Northern Ireland'],
	366 =>	['US', 'USA', '',		'United States of America'],
	367 =>	['US', 'USA', '',		'United States of America'],
	368 =>	['US', 'USA', '',		'United States of America'],
	369 =>	['US', 'USA', '',		'United States of America'],
	370 =>	['PA', 'PAN', '',		'Panama (Republic of)'],
	371 =>	['PA', 'PAN', '',		'Panama (Republic of)'],
	372 =>	['PA', 'PAN', '',		'Panama (Republic of)'],
	373 =>	['PA', 'PAN', '',		'Panama (Republic of)'],
	375 =>	['VC', 'VCT', '',		'Saint Vincent and the Grenadines'],
	376 =>	['VC', 'VCT', '',		'Saint Vincent and the Grenadines'],
	377 =>	['VC', 'VCT', '',		'Saint Vincent and the Grenadines'],
	378	=>	['VG', 'VGB', '',		'British Virgin Islands - United Kingdom of Great Britain and Northern Ireland'],
	379	=>	['VI', 'VIR', '',		'United States Virgin Islands - United States of America'],
	401 =>	['AF', 'AFG', '',		'Afghanistan'],
	403 =>	['SA', 'SAU', '',		'Saudi Arabia (Kingdom of)'],
	405	=>	['BD', 'BGD', '',		'Bangladesh (People\'s Republic of)'],
	408	=>	['BH', 'BHR', '',		'Bahrain (Kingdom of)'],
	410 =>	['BT', 'BTN', '', 		'Bhutan (Kingdom of)'],
	412 =>	['CN', 'CHN', '',		'China (People\'s Republic of)'],
	413 =>	['CN', 'CHN', '',		'China (People\'s Republic of)'],
	414 =>	['CN', 'CHN', '',		'China (People\'s Republic of)'],
	416	=>	['TW', 'TWN', '',		'Taiwan (Province of China) - China (People\'s Republic of)'],
	417	=>	['LK', 'LKA', '',		'Sri Lanka (Democratic Socialist Republic of)'],
	419	=>  ['IN', 'IND', '',		'India (Republic of)'],
	422	=>	['IR', 'IRN', '',		'Iran (Islamic Republic of)'],
	423	=>	['AZ', 'AZE', '',		'Azerbaijan (Republic of)'],
	425	=>	['IQ', 'IRQ', '',		'Iraq (Republic of)'],
	428	=>	['IL', 'ISR', '',		'Israel (State of)'],
	431 =>	['JP', 'JPN', '',		'Japan'],
	432 =>	['JP', 'JPN', '',		'Japan'],
	434	=>	['TM', 'TKM', '',		'Turkmenistan'],
	436	=>	['KZ', 'KAZ', '',		'Kazakhstan (Republic of)'],
	437	=>	['UZ', 'UZB', '',		'Uzbekistan (Republic of)'],
	438	=>	['JO', 'JOR', '',		'Jordan (Hashemite Kingdom of)'],
	440	=>	['KR', 'KOR', '',		'Korea (Republic of)'],
	441	=>	['KR', 'KOR', '',		'Korea (Republic of)'],
	443	=>	['PS', 'PSE', '',		'State of Palestine (In accordance with Resolution 99 Rev. Guadalajara, 2010)'],
	445	=>	['KP', 'PRK', '',		'Democratic People\'s Republic of Korea'],
	447	=>	['KW', 'KWT', '',		'Kuwait (State of)'],
	450	=>	['LB', 'LBN', '',		'Lebanon'],
	451 =>	['KG', 'KGZ', '',		'Kyrgyz Republic'],
	453 =>	['MO', 'MAC', '',		'Macao (Special Administrative Region of China) - China (People\'s Republic of)'],
	455 =>	['MV', 'MDV', '',		'Maldives (Republic of)'],
	457 =>	['MN', 'MNG', '',		'Mongolia'],
	459 =>	['NP', 'NPL', '',		'Nepal (Federal Democratic Republic of)'],
	461 =>	['OM', 'OMN', '',		'Oman (Sultanate of)'],
	463 =>	['PK', 'PAK', '',		'Pakistan (Islamic Republic of)'],
	466 =>	['QA', 'QAT', '',		'Qatar (State of)'],
	468 =>	['SY', 'SYR', '',		'Syrian Arab Republic'],
	470 =>	['AE', 'ARE', '',		'United Arab Emirates'],
	472 =>	['TJ', 'TJK', '',		'Tajikistan (Republic of)'],
	473 =>	['YE', 'YEM', '',		'Yemen (Republic of)'],
	475 =>	['YE', 'YEM', '',		'Yemen (Republic of)'],
	477 =>	['HK', 'HKG', '',		'Hong Kong (Special Administrative Region of China) - China (People\'s Republic of)'],
	478	=>	['BA', 'BIH', '', 		'Bosnia and Herzegovina'],
	501	=>	['FR', 'FRA', 'AQ', 	'Adelie Land - France'],
	503	=>	['AU', 'AUS', '',		'Australia'],
	506 =>	['MM', 'MMR', '',		'Myanmar (Union of)'],
	508 =>	['BN', 'BRN', '',		'Brunei Darussalam'],
	510 =>	['FM', 'FSM', '', 		'Micronesia (Federated States of)'],
	511 =>	['PW', 'PLW', '',		'Palau (Republic of)'],
	512 =>	['NZ', 'NZL', '',		'New Zealand'],
	514 =>	['KH', 'KHM', '',		'Cambodia (Kingdom of)'],
	515 =>	['KH', 'KHM', '',		'Cambodia (Kingdom of)'],
	516 =>	['CX', 'CXR', '',		'Christmas Island (Indian Ocean) - Australia'],
	518 =>	['CK', 'COK', '',		'Cook Islands - New Zealand'],
	520 =>	['FJ', 'FJI', '',		'Fiji (Republic of)'],
	523 =>	['CC', 'CCK', '',		'Cocos (Keeling) Islands - Australia'],
	525 =>	['ID', 'IDN', '',		'Indonesia (Republic of)'],
	529 =>	['KI', 'KIR', '',		'Kiribati (Republic of)'],
	531 =>	['LA', 'LAO', '',		'Lao People\'s Democratic Republic'],
	533 =>	['MY', 'MYS', '',		'Malaysia'],
	536 =>	['MP', 'MNP', '',		'Northern Mariana Islands (Commonwealth of the) - United States of America'],
	538 =>	['MH', 'MHL', '',		'Marshall Islands (Republic of the)'],
	540 =>	['NC', 'NCL', '',		'New Caledonia - France'],
	542 =>	['NU', 'NIU', '',		'Niue - New Zealand'],
	544 =>	['NR', 'NRU', '',		'Nauru (Republic of)'],
	546 =>	['PF', 'PYF', '',		'French Polynesia - France'],
	548 =>	['PH', 'PHL', '',		'Philippines (Republic of the)'],
	553 =>	['PG', 'PNG', '',		'Papua New Guinea'],
	555 =>	['PN', 'PCN', '',		'Pitcairn Island - United Kingdom of Great Britain and Northern Ireland'],
	557 =>	['SB', 'SLB', '',		'Solomon Islands'],
	559 =>	['AS', 'ASM', '',		'American Samoa - United States of America'],
	561 =>	['WS', 'WSM', '',		'Samoa (Independent State of)'],
	563 =>	['SG', 'SGP', '',		'Singapore (Republic of)'],
	564 =>	['SG', 'SGP', '',		'Singapore (Republic of)'],
	565 =>	['SG', 'SGP', '',		'Singapore (Republic of)'],
	566 =>	['SG', 'SGP', '',		'Singapore (Republic of)'],
	567 =>	['TH', 'THA', '',		'Thailand'],
	570	=>	['TO', 'TON', '',		'Tonga (Kingdom of)'],
	572 =>	['TV', 'TUV', '',		'Tuvalu'],
	574 =>	['VN', 'VNM', '', 		'Viet Nam (Socialist Republic of)'],
	576 =>	['VU', 'VUT', '',		'Vanuatu (Republic of)'],
	577 =>	['VU', 'VUT', '',		'Vanuatu (Republic of)'],
	578	=>	['WF', 'WLF', '',		'Wallis and Futuna Islands - France'],
	601	=>	['ZA', 'ZAF', '',		'South Africa (Republic of)'],
	603	=>	['AO', 'AGO', '',		'Angola (Republic of)'],
	605 =>	['DZ', 'DZA', '',		'Algeria (People\'s Democratic Republic of)'],
	607	=>	['FR', 'FRA', 'TF', 	'Saint Paul and Amsterdam Islands - France'],
	608	=>	['GB', 'GBR', 'AC',		'Ascension Island - United Kingdom of Great Britain and Northern Ireland'],
	609 =>	['BI', 'BDI', '',		'Burundi (Republic of)'],
	610 =>	['BJ', 'BEN', '',		'Benin (Republic of)'],
	611	=>	['BW', 'BWA', '',		'Botswana (Republic of)'],
	621	=>	['CF', 'CAF', '',		'Central African Republic'],
	613	=>	['CM', 'CMR', '',		'Cameroon (Republic of)'],
	615	=>	['CG', 'COG', '',		'Congo (Republic of the)'],
	616	=>	['KM', 'COM', '',		'Comoros (Union of the)'],
	617	=>	['CV', 'CPV', '',		'Cabo Verde (Republic of)'],
	618	=>	['FR', 'FRA', 'TF',		'Crozet Archipelago - France'],
	619	=>	['CI', 'CIV', '',		'Ivory Coast (Republic of)'],
	620	=>	['KM', 'COM', '',		'Comoros (Union of the)'],
	621	=>	['DJ', 'DJI', '',		'Djibouti (Republic of)'],
	622	=>  ['EG', 'EGY', '',		'Egypt (Arab Republic of)'],
	624	=>	['ET', 'ETH', '',		'Ethiopia (Federal Democratic Republic of)'],
	625	=>	['ER', 'ERI', '',		'Eritrea'],
	626	=>	['GA', 'GAB', '',		'Gabonese Republic'],
	627	=>	['GH', 'GHA', '',		'Ghana'],
	629	=>	['GM', 'GMB', '',		'Gambia (Republic of the)'],
	630	=>	['GW', 'GNB', '',		'Guinea-Bissau (Republic of)'],
	631	=>	['GQ', 'GNQ', '',		'Equatorial Guinea (Republic of)'],
	632	=>	['GN', 'GIN', '',		'Guinea (Republic of)'],
	633	=>	['BF', 'BFA', '',		'Burkina Faso'],
	634	=>	['KE', 'KEN', '',		'Kenya (Republic of)'],
	635	=>	['FR', 'FRA', 'TF',		'Kerguelen Islands - France'],
	636 =>	['LR', 'LBR', '',		'Liberia (Republic of)'],
	637 =>	['LR', 'LBR', '',		'Liberia (Republic of)'],
	638	=>	['SS', 'SSD', '',		'South Sudan (Republic of)'],
	642	=>	['LY', 'LBY', '',		'Libya'],
	644 =>	['LS', 'LSO', '',		'Lesotho (Kingdom of)'],
	645	=>	['MU', 'MUS', '',		'Mauritius (Republic of)'],
	647 =>	['MG', 'MDG', '',		'Madagascar (Republic of)'],
	649 =>	['ML', 'MLI', '',		'Mali (Republic of)'],
	650 =>	['MZ', 'MOZ', '',		'Mozambique (Republic of)'],
	654 =>	['MR', 'MRT', '',		'Mauritania (Islamic Republic of)'],
	655 =>	['MW', 'MWI', '',		'Malawi (Republic of)'],
	656 =>	['NE', 'NER', '',		'Niger (Republic of the)'],
	656 =>	['NG', 'NGA', '',		'Nigeria (Federal Republic of)'],
	659 =>	['NA', 'NAM', '',		'Namibia (Republic of)'],
	660 =>	['RE', 'REU', '',		'Réunion (French Department of)'],
	661 =>	['RW', 'RWA', '',		'Rwanda (Republic of)'],
	662 =>	['SD', 'SDN', '',		'Sudan (Republic of the)'],
	663 =>	['SN', 'SEN', '',		'Senegal (Republic of)'],
	664 =>	['SC', 'SYC', '',		'Seychelles (Republic of)'],
	665 =>	['SH', 'SHN', '',		'Saint Helena, Ascension and Tristan da Cunha'],
	666 =>	['SO', 'SOM', '',		'Somali Democratic Republic'],
	667 =>	['SL', 'SLE', '',		'Sierra Leone (Republic of)'],
	668 =>	['ST', 'STP', '',		'São Tomé and Príncipe (Democratic Republic of)'],
	669 =>	['SZ', 'SWZ', '',		'Swaziland (Kingdom of)'],
	670 =>	['TD', 'TCD', '',		'Chad (Republic of)'],
	671 =>	['TG', 'TGO', '',		'Togolese Republic'],
	672 =>	['TN', 'TUN', '',		'Tunisian Republic']
}


task :generate_csv do
	puts 'Generating csv...'
	File.open('mids.csv', 'w') do |out|
		data.each do |key, value|
			out.puts ([key] + value).to_csv
		end
	end
end

task :generate_json do
	puts 'Generating json...'
	File.open('mids.json', 'w') do |out|
		out.puts data.to_json
	end
end

task :generate_yaml do
	puts 'Generating yaml...'
	File.open('mids.yaml', 'w') do |out|
		out.puts data.to_yaml
	end
end

# Task for generating markdown for README.md file.
task :generate_markdown do
	puts 'Generating markdown...'
	File.open('mids.md', 'w') do |out|
		out.puts '|    Country     |      Alpha-2    |     Alpha-3     |       MID       |       Flag      |'
		out.puts '| :------------- | :-------------: | :-------------: | :-------------: | :-------------: |'
		data.each do |key,value|
			out.puts "|  #{value[3]} |   #{value[0]} |   #{value[1]} |     #{key}    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/#{value[0].downcase}.png) |"
		end
	end
end

task :default => [:generate_csv, :generate_json, :generate_yaml] do
	puts 'Generating everything...'
end

# TODO: The following entries are to be added.

# 647	Madagascar (Republic of)
# 649	Mali (Republic of)
# 650	Mozambique (Republic of)
# 654	Mauritania (Islamic Republic of)
# 655	Malawi
# 656	Niger (Republic of the)
# 657	Nigeria (Federal Republic of)
# 659	Namibia (Republic of)
# 660	Reunion (French Department of) - France
# 661	Rwanda (Republic of)
# 662	Sudan (Republic of the)
# 663	Senegal (Republic of)
# 664	Seychelles (Republic of)
# 665	Saint Helena - United Kingdom of Great Britain and Northern Ireland
# 666	Somalia (Federal Republic of)
# 667	Sierra Leone
# 668	Sao Tome and Principe (Democratic Republic of)
# 669	Swaziland (Kingdom of)
# 670	Chad (Republic of)
# 671	Togolese Republic
# 672	Tunisia
# 674	Tanzania (United Republic of)
# 675	Uganda (Republic of)
# 676	Democratic Republic of the Congo
# 677	Tanzania (United Republic of)
# 678	Zambia (Republic of)
# 679	Zimbabwe (Republic of)
# 701	Argentine Republic
# 710	Brazil (Federative Republic of)
# 720	Bolivia (Plurinational State of)
# 725	Chile
# 730	Colombia (Republic of)
# 735	Ecuador
# 740	Falkland Islands (Malvinas) - United Kingdom of Great Britain and Northern Ireland
# 745	Guiana (French Department of) - France
# 750	Guyana
# 755	Paraguay (Republic of)
# 760	Peru
# 765	Suriname (Republic of)
# 770	Uruguay (Eastern Republic of)
# 775	Venezuela (Bolivarian Republic of)