Introduction
=================
This project is intended to help map Maritime Identification Digits (MID) to ISO 3166 Country Codes.

What are Maritime Identification Digits?
========================================
Maritime identification digits are used by radio communication facilities to identify their home country or base area in Digital Selective Calling (DSC), Automatic Transmitter Identification System (ATIS), and Automatic Identification System (AIS) messages as part of their Maritime Mobile Service Identities (MMSI).

An MID consists of three digits, always starting with a number from 2 to 7 (assigned regionally) which identifies which country the ship is from. Multiple MIDs can be assigned to a country if it is required. A full listing of MIDs assigned to each country is written in Table 1 of ITU Radio Regulations Appendix 43.

For more information visit [Wikipedia: Maritime Indentification Digits](http://en.wikipedia.org/wiki/Maritime_identification_digits)


Maritime Mobile Service Identity
===========================================
A Maritime Mobile Service Identity (MMSI) is a series of nine digits which are sent in digital form over a radio frequency channel for unique identification. These identities are formed in such a way that the identity or part thereof can be used by telephone and telex subscribers connected to the general telecommunications network to call ships.

For more information visit [Wikipedia: Maritime Mobile Service Identity](http://en.wikipedia.org/wiki/Maritime_Mobile_Service_Identity)

Generating MIDs Mappings
========================
This project uses Ruby to specify the mapping between MID codes and countries. The Rakefile in the root directory contains this information. The following Rake targets can be invoked to generate MIDs mapping files in one of several formats:

- **generate_yaml** YAML output format
- **generate_csv** CSV output format
- **generate_json** JSON output format
- **default** Generates all output formats

Unless contributing to the project, these targets should not need to be invoked as we generate and commit each of the supported mapping formats.

Table of Mapped MID Codes
=========================

|    Country     |      Alpha-2    |     Alpha-3     |       MID       |       Flag      |
| :------------- | :-------------: | :-------------: | :-------------: | :-------------: |
|  Albania (Republic of) |   AL |   ALB |     201    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/al.png) |
|  Andorra (Principality of) |   AD |   AND |     202    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ad.png) |
|  Austria |   AT |   AUT |     203    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/at.png) |
|  Azores - Portugal |   PT |   PRT |     204    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pt.png) |
|  Belgium |   BE |   BEL |     205    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/be.png) |
|  Belarus (Republic of) |   BY |   BLR |     206    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/by.png) |
|  Bulgaria (Republic of) |   BG |   BGR |     207    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bg.png) |
|  Vatican City State |   VA |   VAT |     208    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/va.png) |
|  Cyprus (Republic of) |   CY |   CYP |     209    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cy.png) |
|  Cyprus (Republic of) |   CY |   CYP |     210    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cy.png) |
|  Germany (Federal Republic of) |   DE |   DEU |     211    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/de.png) |
|  Cyprus (Republic of) |   CY |   CYP |     212    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cy.png) |
|  Georgia |   GE |   GEO |     213    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ge.png) |
|  Moldova (Republic of) |   MD |   MDA |     214    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/md.png) |
|  Malta |   MT |   MLT |     215    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mt.png) |
|  Armenia (Republic of) |   AM |   ARM |     216    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/am.png) |
|  Germany (Federal Republic of) |   DE |   DEU |     218    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/de.png) |
|  Denmark |   DK |   DNK |     219    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/dk.png) |
|  Denmark |   DK |   DNK |     220    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/dk.png) |
|  Spain |   ES |   ESP |     224    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/es.png) |
|  Spain |   ES |   ESP |     225    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/es.png) |
|  France |   FR |   FRA |     226    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  France |   FR |   FRA |     227    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  Malta |   MT |   MLT |     228    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mt.png) |
|  Finland |   FI |   FIN |     230    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fi.png) |
|  Faroe Islands - Denmark |   FO |   FRO |     231    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fo.png) |
|  United Kingdom of Great Britain and Northern Ireland |   GB |   GBR |     232    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gb.png) |
|  United Kingdom of Great Britain and Northern Ireland |   GB |   GBR |     233    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gb.png) |
|  United Kingdom of Great Britain and Northern Ireland |   GB |   GBR |     234    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gb.png) |
|  United Kingdom of Great Britain and Northern Ireland |   GB |   GBR |     235    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gb.png) |
|  Gibraltar - United Kingdom of Great Britain and Northern Ireland |   GI |   GIB |     236    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gi.png) |
|  Greece |   GR |   GRC |     237    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gr.png) |
|  Croatia (Republic of) |   HR |   HRV |     238    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/hr.png) |
|  Greece |   GR |   GRC |     239    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gr.png) |
|  Greece |   GR |   GRC |     240    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gr.png) |
|  Greece |   GR |   GRC |     241    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gr.png) |
|  Morocco (Kingdom of) |   MA |   MAR |     242    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ma.png) |
|  Hungary |   HU |   HUN |     243    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/hu.png) |
|  Netherlands (Kingdom of the) |   NL |   NLD |     244    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nl.png) |
|  Netherlands (Kingdom of the) |   NL |   NLD |     245    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nl.png) |
|  Netherlands (Kingdom of the) |   NL |   NLD |     246    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nl.png) |
|  Italy |   IT |   ITA |     247    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/it.png) |
|  Malta |   MT |   MLT |     248    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mt.png) |
|  Ireland |   IE |   IRL |     250    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ie.png) |
|  Iceland |   IS |   ISL |     251    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/is.png) |
|  Liechtenstein (Principality of) |   LI |   LIE |     252    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/li.png) |
|  Luxembourg |   LU |   LUX |     253    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lu.png) |
|  Monaco (Principality of) |   MC |   MCO |     254    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mc.png) |
|  Madeira - Portugal |   PT |   PRT |     255    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pt.png) |
|  Malta |   MT |   MLT |     256    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mt.png) |
|  Norway |   NO |   NOR |     257    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/no.png) |
|  Norway |   NO |   NOR |     258    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/no.png) |
|  Norway |   NO |   NOR |     259    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/no.png) |
|  Poland (Republic of) |   PL |   POL |     261    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pl.png) |
|  Montenegro |   ME |   MNE |     262    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/me.png) |
|  Portugal |   PT |   PRT |     263    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pt.png) |
|  Romania |   RO |   ROU |     264    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ro.png) |
|  Sweden |   SE |   SWE |     265    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/se.png) |
|  Sweden |   SE |   SWE |     266    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/se.png) |
|  Slovak Republic |   SK |   SVK |     267    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sk.png) |
|  San Marino (Republic of) |   SM |   SMR |     268    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sm.png) |
|  Switzerland (Confederation of) |   CH |   CHE |     269    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ch.png) |
|  Czech Republic |   CZ |   CZE |     270    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cz.png) |
|  Turkey |   TR |   TUR |     271    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tr.png) |
|  Ukraine |   UA |   UKR |     272    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ua.png) |
|  Russian Federation |   RU |   RUS |     273    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ru.png) |
|  The Former Yugoslav Republic of Macedonia |   MK |   MKD |     274    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mk.png) |
|  Latvia (Republic of) |   LV |   LVA |     275    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lv.png) |
|  Estonia (Republic of) |   EE |   EST |     276    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ee.png) |
|  Lithuania (Republic of) |   LT |   LTU |     277    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lt.png) |
|  Slovenia (Republic of) |   SI |   SVN |     278    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/si.png) |
|  Serbia (Republic of) |   RS |   SRB |     279    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/rs.png) |
|  Anguilla - United Kingdom of Great Britain and Northern Ireland |   AI |   AIA |     301    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ai.png) |
|  Alaska (State of) - United States of America |   US |   USA |     303    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  Antigua and Barbuda |   AG |   ATG |     304    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ag.png) |
|  Antigua and Barbuda |   AG |   ATG |     305    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ag.png) |
|  Antilles - Netherlands (Kingdom of the) |   CW |   CUW |     306    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cw.png) |
|  Aruba - Netherlands (Kingdom of the) |   AW |   ABW |     307    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/aw.png) |
|  Bahamas (Commonwealth of the) |   BS |   BHS |     308    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bs.png) |
|  Bahamas (Commonwealth of the) |   BS |   BHS |     309    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bs.png) |
|  Bermuda - United Kingdom of Great Britain and Northern Ireland |   BM |   BMU |     310    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bm.png) |
|  Bahamas (Commonwealth of the) |   BS |   BMU |     311    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bs.png) |
|  Belize |   BZ |   BLZ |     312    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bz.png) |
|  Barbados |   BB |   BRB |     314    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bb.png) |
|  Canada |   CA |   CAN |     316    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ca.png) |
|  Cayman Islands - United Kingdom of Great Britain and Northern Ireland |   KY |   CYM |     319    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ky.png) |
|  Costa Rica |   CR |   CRI |     321    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cr.png) |
|  Cuba |   CU |   CUB |     323    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cu.png) |
|  Dominica (Commonwealth of) |   DM |   DMA |     325    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/dm.png) |
|  Dominican Republic |   DO |   DOM |     327    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/do.png) |
|  Guadeloupe (French Department of) - France |   GP |   GLP |     329    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gp.png) |
|  Grenada |   GD |   GRD |     330    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gd.png) |
|  Greenland - Denmark |   GL |   GRL |     331    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gl.png) |
|  Guatemala (Republic of) |   GT |   GTM |     332    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gt.png) |
|  Honduras (Republic of) |   HN |   HND |     335    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/hn.png) |
|  Haiti (Republic of) |   HT |   HTI |     336    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ht.png) |
|  United States of America |   US |   USA |     338    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  Jamaica |   JM |   JAM |     339    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/jm.png) |
|  Saint Kitts and Nevis (Federation of) |   KN |   KNA |     341    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kn.png) |
|  Saint Lucia |   LC |   LCA |     343    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lc.png) |
|  Mexico |   MX |   MEX |     345    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mx.png) |
|  Martinique (French Department of) - France |   MQ |   MTQ |     347    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mq.png) |
|  Montserrat - United Kingdom of Great Britain and Northern Ireland |   MS |   MSR |     348    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ms.png) |
|  Nicaragua |   NI |   NIC |     350    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ni.png) |
|  Panama (Republic of) |   PA |   PAN |     351    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama (Republic of) |   PA |   PAN |     352    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama (Republic of) |   PA |   PAN |     353    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama (Republic of) |   PA |   PAN |     354    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Puerto Rico - United States of America |   PR |   PRI |     358    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pr.png) |
|  El Salvador (Republic of) |   SV |   SLV |     359    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sv.png) |
|  Saint Pierre and Miquelon (Territorial Collectivity of) - France |   PM |   SPM |     361    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pm.png) |
|  Trinidad and Tobago |   TT |   TTO |     362    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tt.png) |
|  Turks and Caicos Islands - United Kingdom of Great Britain and Northern Ireland |   TC |   TCA |     364    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tc.png) |
|  United States of America |   US |   USA |     366    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  United States of America |   US |   USA |     367    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  United States of America |   US |   USA |     368    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  United States of America |   US |   USA |     369    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  Panama (Republic of) |   PA |   PAN |     370    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama (Republic of) |   PA |   PAN |     371    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama (Republic of) |   PA |   PAN |     372    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama (Republic of) |   PA |   PAN |     373    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Saint Vincent and the Grenadines |   VC |   VCT |     375    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vc.png) |
|  Saint Vincent and the Grenadines |   VC |   VCT |     376    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vc.png) |
|  Saint Vincent and the Grenadines |   VC |   VCT |     377    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vc.png) |
|  British Virgin Islands - United Kingdom of Great Britain and Northern Ireland |   VG |   VGB |     378    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vg.png) |
|  United States Virgin Islands - United States of America |   VI |   VIR |     379    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vi.png) |
|  Afghanistan |   AF |   AFG |     401    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/af.png) |
|  Saudi Arabia (Kingdom of) |   SA |   SAU |     403    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sa.png) |
|  Bangladesh (People's Republic of) |   BD |   BGD |     405    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bd.png) |
|  Bahrain (Kingdom of) |   BH |   BHR |     408    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bh.png) |
|  Bhutan (Kingdom of) |   BT |   BTN |     410    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bt.png) |
|  China (People's Republic of) |   CN |   CHN |     412    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cn.png) |
|  China (People's Republic of) |   CN |   CHN |     413    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cn.png) |
|  China (People's Republic of) |   CN |   CHN |     414    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cn.png) |
|  Taiwan (Province of China) - China (People's Republic of) |   TW |   TWN |     416    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tw.png) |
|  Sri Lanka (Democratic Socialist Republic of) |   LK |   LKA |     417    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lk.png) |
|  India (Republic of) |   IN |   IND |     419    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/in.png) |
|  Iran (Islamic Republic of) |   IR |   IRN |     422    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ir.png) |
|  Azerbaijan (Republic of) |   AZ |   AZE |     423    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/az.png) |
|  Iraq (Republic of) |   IQ |   IRQ |     425    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/iq.png) |
|  Israel (State of) |   IL |   ISR |     428    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/il.png) |
|  Japan |   JP |   JPN |     431    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/jp.png) |
|  Japan |   JP |   JPN |     432    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/jp.png) |
|  Turkmenistan |   TM |   TKM |     434    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tm.png) |
|  Kazakhstan (Republic of) |   KZ |   KAZ |     436    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kz.png) |
|  Uzbekistan (Republic of) |   UZ |   UZB |     437    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/uz.png) |
|  Jordan (Hashemite Kingdom of) |   JO |   JOR |     438    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/jo.png) |
|  Korea (Republic of) |   KR |   KOR |     440    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kr.png) |
|  Korea (Republic of) |   KR |   KOR |     441    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kr.png) |
|  State of Palestine (In accordance with Resolution 99 Rev. Guadalajara, 2010) |   PS |   PSE |     443    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ps.png) |
|  Democratic People's Republic of Korea |   KP |   PRK |     445    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kp.png) |
|  Kuwait (State of) |   KW |   KWT |     447    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kw.png) |
|  Lebanon |   LB |   LBN |     450    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lb.png) |
|  Kyrgyz Republic |   KG |   KGZ |     451    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kg.png) |
|  Macao (Special Administrative Region of China) - China (People's Republic of) |   MO |   MAC |     453    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mo.png) |
|  Maldives (Republic of) |   MV |   MDV |     455    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mv.png) |
|  Mongolia |   MN |   MNG |     457    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mn.png) |
|  Nepal (Federal Democratic Republic of) |   NP |   NPL |     459    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/np.png) |
|  Oman (Sultanate of) |   OM |   OMN |     461    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/om.png) |
|  Pakistan (Islamic Republic of) |   PK |   PAK |     463    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pk.png) |
|  Qatar (State of) |   QA |   QAT |     466    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/qa.png) |
|  Syrian Arab Republic |   SY |   SYR |     468    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sy.png) |
|  United Arab Emirates |   AE |   ARE |     470    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ae.png) |
|  Tajikistan (Republic of) |   TJ |   TJK |     472    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tj.png) |
|  Yemen (Republic of) |   YE |   YEM |     473    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ye.png) |
|  Yemen (Republic of) |   YE |   YEM |     475    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ye.png) |
|  Hong Kong (Special Administrative Region of China) - China (People's Republic of) |   HK |   HKG |     477    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/hk.png) |
|  Bosnia and Herzegovina |   BA |   BIH |     478    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ba.png) |
|  Adelie Land - France |   FR |   FRA |     501    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  Australia |   AU |   AUS |     503    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/au.png) |
|  Myanmar (Union of) |   MM |   MMR |     506    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mm.png) |
|  Brunei Darussalam |   BN |   BRN |     508    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bn.png) |
|  Micronesia (Federated States of) |   FM |   FSM |     510    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fm.png) |
|  Palau (Republic of) |   PW |   PLW |     511    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pw.png) |
|  New Zealand |   NZ |   NZL |     512    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nz.png) |
|  Cambodia (Kingdom of) |   KH |   KHM |     514    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kh.png) |
|  Cambodia (Kingdom of) |   KH |   KHM |     515    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kh.png) |
|  Christmas Island (Indian Ocean) - Australia |   CX |   CXR |     516    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cx.png) |
|  Cook Islands - New Zealand |   CK |   COK |     518    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ck.png) |
|  Fiji (Republic of) |   FJ |   FJI |     520    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fj.png) |
|  Cocos (Keeling) Islands - Australia |   CC |   CCK |     523    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cc.png) |
|  Indonesia (Republic of) |   ID |   IDN |     525    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/id.png) |
|  Kiribati (Republic of) |   KI |   KIR |     529    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ki.png) |
|  Lao People's Democratic Republic |   LA |   LAO |     531    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/la.png) |
|  Malaysia |   MY |   MYS |     533    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/my.png) |
|  Northern Mariana Islands (Commonwealth of the) - United States of America |   MP |   MNP |     536    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mp.png) |
|  Marshall Islands (Republic of the) |   MH |   MHL |     538    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mh.png) |
|  New Caledonia - France |   NC |   NCL |     540    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nc.png) |
|  Niue - New Zealand |   NU |   NIU |     542    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nu.png) |
|  Nauru (Republic of) |   NR |   NRU |     544    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nr.png) |
|  French Polynesia - France |   PF |   PYF |     546    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pf.png) |
|  Philippines (Republic of the) |   PH |   PHL |     548    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ph.png) |
|  Papua New Guinea |   PG |   PNG |     553    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pg.png) |
|  Pitcairn Island - United Kingdom of Great Britain and Northern Ireland |   PN |   PCN |     555    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pn.png) |
|  Solomon Islands |   SB |   SLB |     557    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sb.png) |
|  American Samoa - United States of America |   AS |   ASM |     559    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/as.png) |
|  Samoa (Independent State of) |   WS |   WSM |     561    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ws.png) |
|  Singapore (Republic of) |   SG |   SGP |     563    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sg.png) |
|  Singapore (Republic of) |   SG |   SGP |     564    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sg.png) |
|  Singapore (Republic of) |   SG |   SGP |     565    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sg.png) |
|  Singapore (Republic of) |   SG |   SGP |     566    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sg.png) |
|  Thailand |   TH |   THA |     567    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/th.png) |
|  Tonga (Kingdom of) |   TO |   TON |     570    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/to.png) |
|  Tuvalu |   TV |   TUV |     572    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tv.png) |
|  Viet Nam (Socialist Republic of) |   VN |   VNM |     574    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vn.png) |
|  Vanuatu (Republic of) |   VU |   VUT |     576    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vu.png) |
|  Vanuatu (Republic of) |   VU |   VUT |     577    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vu.png) |
|  Wallis and Futuna Islands - France |   WF |   WLF |     578    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/wf.png) |
|  South Africa (Republic of) |   ZA |   ZAF |     601    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/za.png) |
|  Angola (Republic of) |   AO |   AGO |     603    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ao.png) |
|  Algeria (People's Democratic Republic of) |   DZ |   DZA |     605    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/dz.png) |
|  Saint Paul and Amsterdam Islands - France |   FR |   FRA |     607    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  Ascension Island - United Kingdom of Great Britain and Northern Ireland |   GB |   GBR |     608    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gb.png) |
|  Burundi (Republic of) |   BI |   BDI |     609    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bi.png) |
|  Benin (Republic of) |   BJ |   BEN |     610    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bj.png) |
|  Botswana (Republic of) |   BW |   BWA |     611    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bw.png) |
|  Djibouti (Republic of) |   DJ |   DJI |     621    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/dj.png) |
|  Cameroon (Republic of) |   CM |   CMR |     613    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cm.png) |
|  Congo (Republic of the) |   CG |   COG |     615    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cg.png) |
|  Comoros (Union of the) |   KM |   COM |     616    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/km.png) |
|  Cabo Verde (Republic of) |   CV |   CPV |     617    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cv.png) |
|  Crozet Archipelago - France |   FR |   FRA |     618    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  Ivory Coast (Republic of) |   CI |   CIV |     619    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ci.png) |
|  Comoros (Union of the) |   KM |   COM |     620    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/km.png) |
|  Egypt (Arab Republic of) |   EG |   EGY |     622    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/eg.png) |
|  Ethiopia (Federal Democratic Republic of) |   ET |   ETH |     624    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/et.png) |
|  Eritrea |   ER |   ERI |     625    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/er.png) |
|  Gabonese Republic |   GA |   GAB |     626    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ga.png) |
|  Ghana |   GH |   GHA |     627    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gh.png) |
|  Gambia (Republic of the) |   GM |   GMB |     629    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gm.png) |
|  Guinea-Bissau (Republic of) |   GW |   GNB |     630    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gw.png) |
|  Equatorial Guinea (Republic of) |   GQ |   GNQ |     631    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gq.png) |
|  Guinea (Republic of) |   GN |   GIN |     632    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gn.png) |
|  Burkina Faso |   BF |   BFA |     633    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bf.png) |
|  Kenya (Republic of) |   KE |   KEN |     634    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ke.png) |
|  Kerguelen Islands - France |   FR |   FRA |     635    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  Liberia (Republic of) |   LR |   LBR |     636    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lr.png) |
|  Liberia (Republic of) |   LR |   LBR |     637    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lr.png) |
|  South Sudan (Republic of) |   SS |   SSD |     638    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ss.png) |
|  Libya |   LY |   LBY |     642    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ly.png) |
|  Lesotho (Kingdom of) |   LS |   LSO |     644    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ls.png) |
|  Mauritius (Republic of) |   MU |   MUS |     645    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mu.png) |

[_Flags courtesy of Steven Skelton @ flag-icon_](https://github.com/stevenrskelton/flag-icon/)
