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