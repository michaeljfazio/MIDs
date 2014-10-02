require 'json'
require 'yaml'
require 'csv'

# ISO 3166-1			http://en.wikipedia.org/wiki/ISO_3166-1
# ISO 3166-1 alpha-2	http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2
# ISO 3166-1 alpha-3	http://en.wikipedia.org/wiki/ISO_3166-1_alpha-3

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
	254 =>	['MC', 'MCO', '',		'Monaco (Principality of)']
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

task :default => [:generate_csv, :generate_json, :generate_yaml] do
	puts 'Generating everything...'
end

# TODO: The following entries are to be added.

# 255	Madeira - Portugal
# 256	Malta
# 257, 258, 259	Norway
# 261	Poland (Republic of)
# 262	Montenegro
# 263	Portugal
# 264	Romania
# 265, 266	Sweden
# 267	Slovak Republic
# 268	San Marino (Republic of)
# 269	Switzerland (Confederation of)
# 270	Czech Republic
# 271	Turkey
# 272	Ukraine
# 273	Russian Federation
# 274	The Former Yugoslav Republic of Macedonia
# 275	Latvia (Republic of)
# 276	Estonia (Republic of)
# 277	Lithuania (Republic of)	
# 278	Slovenia (Republic of)
# 279	Serbia (Republic of)
# 301	Anguilla - United Kingdom of Great Britain and Northern Ireland
# 303	Alaska (State of) - United States of America
# 304, 305	Antigua and Barbuda
# 306	CuraÁao - Netherlands (Kingdom of the)
# 306	Sint Maarten (Dutch part) - Netherlands (Kingdom of the)
# 306	Bonaire, Sint Eustatius and Saba - Netherlands (Kingdom of the)
# 307	Aruba - Netherlands (Kingdom of the)
# 308, 309	Bahamas (Commonwealth of the)
# 310	Bermuda - United Kingdom of Great Britain and Northern Ireland
# 311	Bahamas (Commonwealth of the)
# 312	Belize
# 314	Barbados
# 316	Canada
# 319	Cayman Islands - United Kingdom of Great Britain and Northern Ireland
# 321	Costa Rica
# 323	Cuba
# 325	Dominica (Commonwealth of)
# 327	Dominican Republic
# 329	Guadeloupe (French Department of) - France
# 330	Grenada
# 331	Greenland - Denmark
# 332	Guatemala (Republic of)
# 334	Honduras (Republic of)
# 336	Haiti (Republic of)
# 338	United States of America
# 339	Jamaica
# 341	Saint Kitts and Nevis (Federation of)
# 343	Saint Lucia
# 345	Mexico
# 347	Martinique (French Department of) - France
# 348	Montserrat - United Kingdom of Great Britain and Northern Ireland
# 350	Nicaragua
# 351, 352, 353, 354	Panama (Republic of)
# 355,356, 357	-
# 358	Puerto Rico - United States of America
# 359	El Salvador (Republic of)
# 361	Saint Pierre and Miquelon (Territorial Collectivity of) - France
# 362	Trinidad and Tobago
# 364	Turks and Caicos Islands - United Kingdom of Great Britain and Northern Ireland
# 366, 367, 368, 369	United States of America
# 370, 371, 372, 373	Panama (Republic of)
# 375, 376, 377	Saint Vincent and the Grenadines
# 378	British Virgin Islands - United Kingdom of Great Britain and Northern Ireland
# 379	United States Virgin Islands - United States of America
# 401	Afghanistan
# 403	Saudi Arabia (Kingdom of)
# 405	Bangladesh (People's Republic of)
# 408	Bahrain (Kingdom of)
# 410	Bhutan (Kingdom of)
# 412, 413, 414	China (People's Republic of)
# 416	Taiwan (Province of China) - China (People's Republic of)
# 417	Sri Lanka (Democratic Socialist Republic of)
# 419	India (Republic of)
# 422	Iran (Islamic Republic of)
# 423	Azerbaijan (Republic of)
# 425	Iraq (Republic of)
# 428	Israel (State of)
# 431, 432	Japan
# 434	Turkmenistan
# 436	Kazakhstan (Republic of)
# 437	Uzbekistan (Republic of)
# 438	Jordan (Hashemite Kingdom of)
# 440, 441	Korea (Republic of)
# 443	State of Palestine (In accordance with Resolution 99 Rev. Guadalajara, 2010)
# 445	Democratic People's Republic of Korea
# 447	Kuwait (State of)
# 450	Lebanon
# 451	Kyrgyz Republic
# 453	Macao (Special Administrative Region of China) - China (People's Republic of)
# 455	Maldives (Republic of)
# 457	Mongolia
# 459	Nepal (Federal Democratic Republic of)
# 461	Oman (Sultanate of)
# 463	Pakistan (Islamic Republic of)
# 466	Qatar (State of)
# 468	Syrian Arab Republic
# 470	United Arab Emirates
# 472	Tajikistan (Republic of)
# 473, 475	Yemen (Republic of)
# 477	Hong Kong (Special Administrative Region of China) - China (People's Republic of)
# 478	Bosnia and Herzegovina
# 501	Adelie Land - France
# 503	Australia
# 506	Myanmar (Union of)
# 508	Brunei Darussalam
# 510	Micronesia (Federated States of)
# 511	Palau (Republic of)
# 512	New Zealand
# 514, 515	Cambodia (Kingdom of)
# 516	Christmas Island (Indian Ocean) - Australia
# 518	Cook Islands - New Zealand
# 520	Fiji (Republic of)
# 523	Cocos (Keeling) Islands - Australia
# 525	Indonesia (Republic of)
# 529	Kiribati (Republic of)
# 531	Lao People's Democratic Republic
# 533	Malaysia
# 536	Northern Mariana Islands (Commonwealth of the) - United States of America
# 538	Marshall Islands (Republic of the)
# 540	New Caledonia - France
# 542	Niue - New Zealand
# 544	Nauru (Republic of)
# 546	French Polynesia - France
# 548	Philippines (Republic of the)
# 553	Papua New Guinea
# 555	Pitcairn Island - United Kingdom of Great Britain and Northern Ireland
# 557	Solomon Islands
# 559	American Samoa - United States of America
# 561	Samoa (Independent State of)
# 563, 564, 565, 566	Singapore (Republic of)
# 567	Thailand
# 570	Tonga (Kingdom of)
# 572	Tuvalu
# 574	Viet Nam (Socialist Republic of)
# 576, 577	Vanuatu (Republic of)
# 578	Wallis and Futuna Islands - France
# 601	South Africa (Republic of)
# 603	Angola (Republic of)
# 605	Algeria (People's Democratic Republic of)
# 607	Saint Paul and Amsterdam Islands - France
# 608	Ascension Island - United Kingdom of Great Britain and Northern Ireland
# 609	Burundi (Republic of)
# 610	Benin (Republic of)
# 611	Botswana (Republic of)
# 612	Central African Republic
# 613	Cameroon (Republic of)
# 615	Congo (Republic of the)
# 616	Comoros (Union of the)
# 617	Cabo Verde (Republic of)
# 618	Crozet Archipelago - France
# 619	CÙte d'Ivoire (Republic of)
# 620	Comoros (Union of the)
# 621	Djibouti (Republic of)
# 622	Egypt (Arab Republic of)
# 624	Ethiopia (Federal Democratic Republic of)
# 625	Eritrea
# 626	Gabonese Republic
# 627	Ghana
# 629	Gambia (Republic of the)
# 630	Guinea-Bissau (Republic of)
# 631	Equatorial Guinea (Republic of)
# 632	Guinea (Republic of)
# 633	Burkina Faso
# 634	Kenya (Republic of)
# 635	Kerguelen Islands - France
# 636, 637	Liberia (Republic of)
# 638	South Sudan (Republic of)
# 642	Libya
# 644	Lesotho (Kingdom of)
# 645	Mauritius (Republic of)
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