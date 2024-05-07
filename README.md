# TRANSCEND Project survey data cleaning for Jakarta

## Description
This repo includes the code used for data cleaning and preparation in the [TRANSCEND Project](https://www.transcend-project.org). Specifically, it includes the procedures and data for the Jakarta case study, developed with local partners.

## Goal
This repo provides open access to the source code using when manipulating the fieldwork data, providing accountability and traceability of all changes we implemented. This seeks to provide outside validation to the procedures we implemented, and minimize human or procedural errors in the data manipulation.

## Usage
Sync the data cleaning scripts to this repo when meaningful. Use branches to test new features before committing them to the main.

## Support
Reach out to our team: 
- alexandre.santos(at)lmu.de
- c.mirbach(at)lmu.de

## Roadmap
1. Synthesize the data-cleaning applications from Mumbai for reuse
2. Merge the Baratha-Indonesia survey responses with the English data-dictionary
3. Implement data-cleaning procedures, including at least [source:](https://towardsdatascience.com/the-ultimate-guide-to-data-cleaning-3969843991d4):
- Data-Type Constraints: values in a particular column must be of a particular datatype, e.g., boolean, numeric, date, etc.
- Range Constraints: typically, numbers or dates should fall within a certain range.
- Mandatory Constraints: certain columns cannot be empty.
- Unique Constraints: a field, or a combination of fields, must be unique across a dataset.
- Set-Membership constraints: values of a column come from a set of discrete values, e.g. enum 3.6 values. For example, a person’s gender may be male or female.
- Foreign-key constraints: as in relational databases, a foreign key column can’t have a value that does not exist in the referenced primary key.
- Regular expression patterns: text fields that have to be in a certain pattern. For example, phone numbers may be required to have the pattern (999) 999–9999.
- Cross-field validation: certain conditions that span across multiple fields must hold. For example, a patient’s date of discharge from the hospital cannot be earlier than the date of admission.

## Authors and acknowledgment
Dr. Alexandre Pereira Santos
Charlota Mirbach
Jingyao Zhou

## Project status
Ongoing.