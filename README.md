Introduction
=================
This project is intended to help map Maritime Identification Digits (MID) to ISO 3166 Country Codes.

Using MIDs with Bower
=====================
If your project is using [bower](http://bower.io), then you can add MIDs as a dependency by invoking the following command:

```shell
bower install mids --save
```

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
|  Albania |   AL |   ALB |     201    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/al.png) |
|  Andorra |   AD |   AND |     202    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ad.png) |
|  Austria |   AT |   AUT |     203    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/at.png) |
|  Azores |   PT |   PRT |     204    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pt.png) |
|  Belgium |   BE |   BEL |     205    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/be.png) |
|  Belarus |   BY |   BLR |     206    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/by.png) |
|  Bulgaria |   BG |   BGR |     207    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bg.png) |
|  Vatican City State |   VA |   VAT |     208    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/va.png) |
|  Cyprus |   CY |   CYP |     209    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cy.png) |
|  Cyprus |   CY |   CYP |     210    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cy.png) |
|  Germany |   DE |   DEU |     211    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/de.png) |
|  Cyprus |   CY |   CYP |     212    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cy.png) |
|  Georgia |   GE |   GEO |     213    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ge.png) |
|  Moldova |   MD |   MDA |     214    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/md.png) |
|  Malta |   MT |   MLT |     215    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mt.png) |
|  Armenia |   AM |   ARM |     216    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/am.png) |
|  Germany |   DE |   DEU |     218    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/de.png) |
|  Denmark |   DK |   DNK |     219    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/dk.png) |
|  Denmark |   DK |   DNK |     220    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/dk.png) |
|  Spain |   ES |   ESP |     224    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/es.png) |
|  Spain |   ES |   ESP |     225    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/es.png) |
|  France |   FR |   FRA |     226    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  France |   FR |   FRA |     227    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  Malta |   MT |   MLT |     228    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mt.png) |
|  Finland |   FI |   FIN |     230    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fi.png) |
|  Faroe Islands |   FO |   FRO |     231    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fo.png) |
|  United Kingdom |   GB |   GBR |     232    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gb.png) |
|  United Kingdom |   GB |   GBR |     233    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gb.png) |
|  United Kingdom |   GB |   GBR |     234    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gb.png) |
|  United Kingdom |   GB |   GBR |     235    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gb.png) |
|  Gibraltar |   GI |   GIB |     236    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gi.png) |
|  Greece |   GR |   GRC |     237    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gr.png) |
|  Croatia |   HR |   HRV |     238    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/hr.png) |
|  Greece |   GR |   GRC |     239    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gr.png) |
|  Greece |   GR |   GRC |     240    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gr.png) |
|  Greece |   GR |   GRC |     241    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gr.png) |
|  Morocco |   MA |   MAR |     242    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ma.png) |
|  Hungary |   HU |   HUN |     243    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/hu.png) |
|  Netherlands |   NL |   NLD |     244    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nl.png) |
|  Netherlands |   NL |   NLD |     245    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nl.png) |
|  Netherlands |   NL |   NLD |     246    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nl.png) |
|  Italy |   IT |   ITA |     247    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/it.png) |
|  Malta |   MT |   MLT |     248    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mt.png) |
|  Ireland |   IE |   IRL |     250    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ie.png) |
|  Iceland |   IS |   ISL |     251    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/is.png) |
|  Liechtenstein |   LI |   LIE |     252    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/li.png) |
|  Luxembourg |   LU |   LUX |     253    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lu.png) |
|  Monaco |   MC |   MCO |     254    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mc.png) |
|  Madeira |   PT |   PRT |     255    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pt.png) |
|  Malta |   MT |   MLT |     256    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mt.png) |
|  Norway |   NO |   NOR |     257    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/no.png) |
|  Norway |   NO |   NOR |     258    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/no.png) |
|  Norway |   NO |   NOR |     259    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/no.png) |
|  Poland |   PL |   POL |     261    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pl.png) |
|  Montenegro |   ME |   MNE |     262    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/me.png) |
|  Portugal |   PT |   PRT |     263    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pt.png) |
|  Romania |   RO |   ROU |     264    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ro.png) |
|  Sweden |   SE |   SWE |     265    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/se.png) |
|  Sweden |   SE |   SWE |     266    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/se.png) |
|  Slovak Republic |   SK |   SVK |     267    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sk.png) |
|  San Marino |   SM |   SMR |     268    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sm.png) |
|  Switzerland |   CH |   CHE |     269    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ch.png) |
|  Czech Republic |   CZ |   CZE |     270    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cz.png) |
|  Turkey |   TR |   TUR |     271    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tr.png) |
|  Ukraine |   UA |   UKR |     272    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ua.png) |
|  Russia |   RU |   RUS |     273    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ru.png) |
|  Macedonia |   MK |   MKD |     274    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mk.png) |
|  Latvia |   LV |   LVA |     275    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lv.png) |
|  Estonia |   EE |   EST |     276    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ee.png) |
|  Lithuania |   LT |   LTU |     277    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lt.png) |
|  Slovenia |   SI |   SVN |     278    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/si.png) |
|  Serbia |   RS |   SRB |     279    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/rs.png) |
|  Anguilla |   AI |   AIA |     301    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ai.png) |
|  Alaska |   US |   USA |     303    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  Antigua and Barbuda |   AG |   ATG |     304    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ag.png) |
|  Antigua and Barbuda |   AG |   ATG |     305    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ag.png) |
|  Antilles |   CW |   CUW |     306    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cw.png) |
|  Aruba |   AW |   ABW |     307    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/aw.png) |
|  Bahamas |   BS |   BHS |     308    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bs.png) |
|  Bahamas |   BS |   BHS |     309    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bs.png) |
|  Bermuda |   BM |   BMU |     310    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bm.png) |
|  Bahamas |   BS |   BMU |     311    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bs.png) |
|  Belize |   BZ |   BLZ |     312    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bz.png) |
|  Barbados |   BB |   BRB |     314    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bb.png) |
|  Canada |   CA |   CAN |     316    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ca.png) |
|  Cayman Islands |   KY |   CYM |     319    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ky.png) |
|  Costa Rica |   CR |   CRI |     321    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cr.png) |
|  Cuba |   CU |   CUB |     323    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cu.png) |
|  Dominica |   DM |   DMA |     325    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/dm.png) |
|  Dominican Republic |   DO |   DOM |     327    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/do.png) |
|  Guadeloupe |   GP |   GLP |     329    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gp.png) |
|  Grenada |   GD |   GRD |     330    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gd.png) |
|  Greenland |   GL |   GRL |     331    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gl.png) |
|  Guatemala |   GT |   GTM |     332    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gt.png) |
|  Honduras |   HN |   HND |     335    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/hn.png) |
|  Haiti |   HT |   HTI |     336    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ht.png) |
|  United States of America |   US |   USA |     338    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  Jamaica |   JM |   JAM |     339    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/jm.png) |
|  Saint Kitts and Nevis |   KN |   KNA |     341    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kn.png) |
|  Saint Lucia |   LC |   LCA |     343    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lc.png) |
|  Mexico |   MX |   MEX |     345    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mx.png) |
|  Martinique |   MQ |   MTQ |     347    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mq.png) |
|  Montserrat |   MS |   MSR |     348    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ms.png) |
|  Nicaragua |   NI |   NIC |     350    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ni.png) |
|  Panama |   PA |   PAN |     351    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama |   PA |   PAN |     352    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama |   PA |   PAN |     353    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama |   PA |   PAN |     354    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Puerto Rico |   PR |   PRI |     358    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pr.png) |
|  El Salvador |   SV |   SLV |     359    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sv.png) |
|  Saint Pierre and Miquelon |   PM |   SPM |     361    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pm.png) |
|  Trinidad and Tobago |   TT |   TTO |     362    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tt.png) |
|  Turks and Caicos Islands |   TC |   TCA |     364    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tc.png) |
|  United States of America |   US |   USA |     366    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  United States of America |   US |   USA |     367    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  United States of America |   US |   USA |     368    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  United States of America |   US |   USA |     369    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/us.png) |
|  Panama |   PA |   PAN |     370    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama |   PA |   PAN |     371    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama |   PA |   PAN |     372    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Panama |   PA |   PAN |     373    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pa.png) |
|  Saint Vincent and the Grenadines |   VC |   VCT |     375    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vc.png) |
|  Saint Vincent and the Grenadines |   VC |   VCT |     376    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vc.png) |
|  Saint Vincent and the Grenadines |   VC |   VCT |     377    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vc.png) |
|  British Virgin Islands |   VG |   VGB |     378    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vg.png) |
|  United States Virgin Islands |   VI |   VIR |     379    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vi.png) |
|  Afghanistan |   AF |   AFG |     401    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/af.png) |
|  Saudi Arabia |   SA |   SAU |     403    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sa.png) |
|  Bangladesh |   BD |   BGD |     405    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bd.png) |
|  Bahrain |   BH |   BHR |     408    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bh.png) |
|  Bhutan |   BT |   BTN |     410    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bt.png) |
|  China |   CN |   CHN |     412    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cn.png) |
|  China |   CN |   CHN |     413    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cn.png) |
|  China |   CN |   CHN |     414    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cn.png) |
|  Taiwan |   TW |   TWN |     416    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tw.png) |
|  Sri Lanka |   LK |   LKA |     417    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lk.png) |
|  India |   IN |   IND |     419    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/in.png) |
|  Iran |   IR |   IRN |     422    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ir.png) |
|  Azerbaijan |   AZ |   AZE |     423    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/az.png) |
|  Iraq |   IQ |   IRQ |     425    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/iq.png) |
|  Israel |   IL |   ISR |     428    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/il.png) |
|  Japan |   JP |   JPN |     431    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/jp.png) |
|  Japan |   JP |   JPN |     432    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/jp.png) |
|  Turkmenistan |   TM |   TKM |     434    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tm.png) |
|  Kazakhstan |   KZ |   KAZ |     436    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kz.png) |
|  Uzbekistan |   UZ |   UZB |     437    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/uz.png) |
|  Jordan |   JO |   JOR |     438    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/jo.png) |
|  Korea |   KR |   KOR |     440    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kr.png) |
|  Korea |   KR |   KOR |     441    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kr.png) |
|  State of Palestine |   PS |   PSE |     443    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ps.png) |
|  Democratic People's Republic of Korea |   KP |   PRK |     445    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kp.png) |
|  Kuwait |   KW |   KWT |     447    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kw.png) |
|  Lebanon |   LB |   LBN |     450    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lb.png) |
|  Kyrgyz Republic |   KG |   KGZ |     451    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kg.png) |
|  Macao |   MO |   MAC |     453    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mo.png) |
|  Maldives |   MV |   MDV |     455    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mv.png) |
|  Mongolia |   MN |   MNG |     457    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mn.png) |
|  Nepal |   NP |   NPL |     459    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/np.png) |
|  Oman |   OM |   OMN |     461    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/om.png) |
|  Pakistan |   PK |   PAK |     463    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pk.png) |
|  Qatar (State of) |   QA |   QAT |     466    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/qa.png) |
|  Syrian Arab Republic |   SY |   SYR |     468    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sy.png) |
|  United Arab Emirates |   AE |   ARE |     470    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ae.png) |
|  Tajikistan |   TJ |   TJK |     472    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tj.png) |
|  Yemen |   YE |   YEM |     473    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ye.png) |
|  Yemen |   YE |   YEM |     475    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ye.png) |
|  Hong Kong |   HK |   HKG |     477    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/hk.png) |
|  Bosnia and Herzegovina |   BA |   BIH |     478    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ba.png) |
|  Adelie Land |   FR |   FRA |     501    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  Australia |   AU |   AUS |     503    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/au.png) |
|  Myanmar |   MM |   MMR |     506    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mm.png) |
|  Brunei Darussalam |   BN |   BRN |     508    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bn.png) |
|  Micronesia |   FM |   FSM |     510    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fm.png) |
|  Palau |   PW |   PLW |     511    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pw.png) |
|  New Zealand |   NZ |   NZL |     512    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nz.png) |
|  Cambodia |   KH |   KHM |     514    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kh.png) |
|  Cambodia |   KH |   KHM |     515    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/kh.png) |
|  Christmas Island |   CX |   CXR |     516    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cx.png) |
|  Cook Islands |   CK |   COK |     518    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ck.png) |
|  Fiji |   FJ |   FJI |     520    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fj.png) |
|  Cocos (Keeling) Islands |   CC |   CCK |     523    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cc.png) |
|  Indonesia |   ID |   IDN |     525    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/id.png) |
|  Kiribati |   KI |   KIR |     529    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ki.png) |
|  Lao People's Democratic Republic |   LA |   LAO |     531    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/la.png) |
|  Malaysia |   MY |   MYS |     533    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/my.png) |
|  Northern Mariana Islands |   MP |   MNP |     536    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mp.png) |
|  Marshall Islands |   MH |   MHL |     538    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mh.png) |
|  New Caledonia |   NC |   NCL |     540    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nc.png) |
|  Niue |   NU |   NIU |     542    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nu.png) |
|  Nauru |   NR |   NRU |     544    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/nr.png) |
|  French Polynesia |   PF |   PYF |     546    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pf.png) |
|  Philippines |   PH |   PHL |     548    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ph.png) |
|  Papua New Guinea |   PG |   PNG |     553    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pg.png) |
|  Pitcairn Island |   PN |   PCN |     555    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pn.png) |
|  Solomon Islands |   SB |   SLB |     557    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sb.png) |
|  American Samoa |   AS |   ASM |     559    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/as.png) |
|  Samoa |   WS |   WSM |     561    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ws.png) |
|  Singapore |   SG |   SGP |     563    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sg.png) |
|  Singapore |   SG |   SGP |     564    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sg.png) |
|  Singapore |   SG |   SGP |     565    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sg.png) |
|  Singapore |   SG |   SGP |     566    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sg.png) |
|  Thailand |   TH |   THA |     567    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/th.png) |
|  Tonga |   TO |   TON |     570    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/to.png) |
|  Tuvalu |   TV |   TUV |     572    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tv.png) |
|  Viet Nam |   VN |   VNM |     574    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vn.png) |
|  Vanuatu |   VU |   VUT |     576    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vu.png) |
|  Vanuatu |   VU |   VUT |     577    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/vu.png) |
|  Wallis and Futuna Islands |   WF |   WLF |     578    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/wf.png) |
|  South Africa |   ZA |   ZAF |     601    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/za.png) |
|  Angola |   AO |   AGO |     603    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ao.png) |
|  Algeria |   DZ |   DZA |     605    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/dz.png) |
|  Saint Paul and Amsterdam Islands |   FR |   FRA |     607    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  Ascension Island |   GB |   GBR |     608    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gb.png) |
|  Burundi |   BI |   BDI |     609    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bi.png) |
|  Benin |   BJ |   BEN |     610    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bj.png) |
|  Botswana |   BW |   BWA |     611    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bw.png) |
|  Djibouti |   DJ |   DJI |     621    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/dj.png) |
|  Cameroon |   CM |   CMR |     613    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cm.png) |
|  Congo |   CG |   COG |     615    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cg.png) |
|  Comoros |   KM |   COM |     616    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/km.png) |
|  Cabo Verde |   CV |   CPV |     617    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cv.png) |
|  Crozet Archipelago |   FR |   FRA |     618    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  Ivory Coast |   CI |   CIV |     619    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ci.png) |
|  Comoros |   KM |   COM |     620    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/km.png) |
|  Egypt |   EG |   EGY |     622    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/eg.png) |
|  Ethiopia |   ET |   ETH |     624    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/et.png) |
|  Eritrea |   ER |   ERI |     625    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/er.png) |
|  Gabonese Republic |   GA |   GAB |     626    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ga.png) |
|  Ghana |   GH |   GHA |     627    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gh.png) |
|  Gambia |   GM |   GMB |     629    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gm.png) |
|  Guinea-Bissau |   GW |   GNB |     630    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gw.png) |
|  Equatorial Guinea |   GQ |   GNQ |     631    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gq.png) |
|  Guinea |   GN |   GIN |     632    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gn.png) |
|  Burkina Faso |   BF |   BFA |     633    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bf.png) |
|  Kenya |   KE |   KEN |     634    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ke.png) |
|  Kerguelen Islands |   FR |   FRA |     635    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fr.png) |
|  Liberia |   LR |   LBR |     636    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lr.png) |
|  Liberia |   LR |   LBR |     637    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/lr.png) |
|  South Sudan |   SS |   SSD |     638    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ss.png) |
|  Libya |   LY |   LBY |     642    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ly.png) |
|  Lesotho |   LS |   LSO |     644    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ls.png) |
|  Mauritius |   MU |   MUS |     645    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mu.png) |
|  Madagascar |   MG |   MDG |     647    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mg.png) |
|  Mali |   ML |   MLI |     649    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ml.png) |
|  Mozambique |   MZ |   MOZ |     650    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mz.png) |
|  Mauritania |   MR |   MRT |     654    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mr.png) |
|  Malawi |   MW |   MWI |     655    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/mw.png) |
|  Nigeria |   NG |   NGA |     656    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ng.png) |
|  Namibia |   NA |   NAM |     659    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/na.png) |
|  Reunion |   RE |   REU |     660    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/re.png) |
|  Rwanda |   RW |   RWA |     661    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/rw.png) |
|  Sudan |   SD |   SDN |     662    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sd.png) |
|  Senegal |   SN |   SEN |     663    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sn.png) |
|  Seychelles |   SC |   SYC |     664    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sc.png) |
|  Saint Helena |   SH |   SHN |     665    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sh.png) |
|  Somali Democratic Republic |   SO |   SOM |     666    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/so.png) |
|  Sierra Leone |   SL |   SLE |     667    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sl.png) |
|  Sao Tome and Principe |   ST |   STP |     668    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/st.png) |
|  Swaziland |   SZ |   SWZ |     669    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sz.png) |
|  Chad |   TD |   TCD |     670    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/td.png) |
|  Togolese Republic |   TG |   TGO |     671    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tg.png) |
|  Tunisian Republic |   TN |   TUN |     672    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tn.png) |
|  Tanzania |   TZ |   TZA |     674    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tz.png) |
|  Uganda |   UG |   UGA |     675    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ug.png) |
|  Democratic Republic of the Congo |   CD |   COD |     676    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cd.png) |
|  Tanzania |   TZ |   TZA |     677    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/tz.png) |
|  Zambia |   ZM |   ZMB |     678    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/zm.png) |
|  Zimbabwe |   ZW |   ZWE |     679    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/zw.png) |
|  Argentine Republic |   AR |   ARG |     701    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ar.png) |
|  Brazil |   BR |   BRA |     710    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/br.png) |
|  Bolivia |   BO |   BOL |     720    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/bo.png) |
|  Chile |   CL |   CHL |     725    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/cl.png) |
|  Colombia |   CO |   COL |     730    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/co.png) |
|  Ecuador |   EC |   ECU |     735    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ec.png) |
|  Falkland Islands |   FK |   FLK |     740    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/fk.png) |
|  Guiana |   GF |   GUF |     745    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gf.png) |
|  Guyana |   GY |   GUY |     750    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/gy.png) |
|  Paraguay |   PY |   PRY |     755    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/py.png) |
|  Peru |   PE |   PER |     760    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/pe.png) |
|  Suriname |   SR |   SUR |     765    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/sr.png) |
|  Uruguay |   UY |   URY |     770    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/uy.png) |
|  Venezuela |   VE |   VEN |     775    | ![](https://raw.githubusercontent.com/stevenrskelton/flag-icon/master/png/16/country-4x3/ve.png) |


[_Flags courtesy of Steven Skelton @ flag-icon_](https://github.com/stevenrskelton/flag-icon/)
