# automation
# Python 401d1818
## Labs 19: Automation
### Authors: Steve Ngo
​
## Overview
Filter through a txt file and return emails and phone numbers

## Feature Tasks and Requirements
* Given a document `potential-contacts`, find and collect all email addresses and phone numbers.
* Phone numbers may be in various formats.
  * (xxx) yyy-zzzz, yyy-zzzz, xxx-yyy-zzzz, etc.
  * phone numbers with missing area code should presume 206
  * phone numbers should be stored in xxx-yyy-zzzz format.
* Once emails and phone numbers are found they should be stored in two separate documents.
* The information should be sorted in ascending order.
* Duplicate entries are not allowed.

## Implementation Notes:
* Find `potential-contacts.txt` and `existing-contacts`.txt in folder `assets` for today’s class in course repo.

## Example:
### phone_numbers.txt
```
123-456-7890
206-678-9012
234-567-8901
```

### emails.txt
```
ana@foo.bar
bill_x@foo.bar
chris.schmidt@bar.baz
```

## Stretch:
* It turns out some of the contacts are already in our system.
  * Compare your collected data against `existing-contacts`.txt and only include info NOT already in system.
* Handle phone numbers with extensions. E.g. (123) 456-789x012

## Setup

```
python3 -m venv .venv 
source .venv/bin/activate

pip install pytest
pip freeze > requirements.txt

cat requirements.txt 
pip install -r requirements.txt
pip install --upgrade pip

pytest
```