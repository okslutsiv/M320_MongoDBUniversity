# Lab: Apply the Computed Pattern

**Problem**:

User Story

Our city is going green, and we're reassessing our power plant. A lot of residents are switching to solar panels for their source of electricity and the power plant needs to be both ecologically friendly and flexible in its distribution of electricity throughout the city.

A number of residents are on board with the Green New Deal and are promptly installing solar panels on their homes, which reduces the consumption of electricity from the power plant.

In some cases, the new solar homes produce more energy than they use, thus selling the excess energy back to the power plant.

Our database is tracking the following data about each building in the city: how much energy in kilowatts (kW) per hour it produces (if any), how much energy it consumes, and how much energy needs to be supplemented daily.

In order to make our plant more flexible in adapting to the growing number of solar-powered homes and to project out to the happy date when there won't be a need for a city power plant, our computer algorithms are analyzing consumption data by city zones one day at a time.

```javascript
{
  "_id": ObjectId("5c9414f25e6aff2b8870a2d0"),
  "address": {
    "building number": "742",
    "street name": "Evergreen Terrace",
    "city": "Springfield",
    "state": "MA",
    "zip code": "01111"
  },
  "owner": "Homer J. Simpson",
  "zone": 13,
  "date": ISODate("2019-03-21T23:03:31.197Z"),
  "kW per day": {
    "consumption": 10,
    "self-produced": 7,
    "city-supplemented": 3
  }
}
```

The problem with this design is that we need to calculate zone totals from each building's report every day, which is a lot of unnecessary calculation during reads.

Every zone has anywhere from 100 to 900 buildings and we will create a zone collection using the consumption data that comes in from every unit in each zone daily.

**Task**

To address this issue, we've decided to implement the Computed Pattern. We will create a separate collection that stores zone-based summaries on zone consumption, production, and city-supplemented energy metrics, which we will calculate and overwrite whenever new data comes into the system.

To complete this lab:

Modify the following schema to represent the schema we will store in our computed collection. Remove any fields we do not need to store in our computed collection:

```javascript
{
  "_id": "<objectId>",
  "address": {
    "building number": "<string>",
    "street name": "<string>",
    "city": "<string>",
    "state": "<string>",
    "zip code": "<string>"
  },
  "owner": "<string>",
  "zone": "<int>",
  "date": "<date>",
  "kW per day": {
    "consumption": "<int>",
    "self-produced": "<int>",
    "city-supplemented": "<int>"
  }
}
```

Save the updated schema to a file named pattern_computed.json.

Validate your answer on Windows by running in the CMD shell:

```javascript
validate_m320 pattern_computed --file pattern_computed.json
```

Validate your answer on MacOS and Linux by running:

```javascript
./validate_m320 pattern_computed --file pattern_computed.json
```

After running this script, you will either be given a validation code or an error message indicating what might be missing in your file.

When you get the validation code paste it in the text box below and click submit.

Attempts Remaining:3 Attempts left

Enter answer here:

**5c94f393f752ec6b191c3c7d**
