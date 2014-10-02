MIDS
====

Maritime Identification Digits Mapping to Country Codes

Rake targets necessary to generate the MIDs mappings 
- generate_yaml
- generate_csv
- generate_json

Maritime identification digits are used by radio communication facilities to identify their home country or base area in Digital Selective Calling (DSC), Automatic Transmitter Identification System (ATIS), and Automatic Identification System (AIS) messages as part of their Maritime Mobile Service Identities.

An MID consists of three digits, always starting with a number from 2 to 7 (assigned regionally). A second MID can be assigned once the first or subsequently allocated MID is more than 80% exhausted, and the rate of assignments is such that 90% exhaustion is foreseen. A listing of MIDs assigned to each country is written in Table 1 of ITU Radio Regulations Appendix 43.

A quick over view is at [Wikipedia: Maritime Indentification Digits](http://en.wikipedia.org/wiki/Maritime_identification_digits)



A Maritime Mobile Service Identity (MMSI) is a series of nine digits which are sent in digital form over a radio frequency channel in order to uniquely identify ship stations, ship earth stations, coast stations, coast earth stations, and group calls. These identities are formed in such a way that the identity or part thereof can be used by telephone and telex subscribers connected to the general telecommunications network to call ships automatically.

A quick over view is at [Wikipedia: Maritime Mobile Service Identity](http://en.wikipedia.org/wiki/Maritime_Mobile_Service_Identity)


This project is intended to map MIDs to ISO country codes.
