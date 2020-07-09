<p align="center">
  <img src="https://yalewkidane.github.io/cityhub-data-model/images/cityhubs.png">
</p>

<p align="center">
  <img src="https://yalewkidane.github.io/cityhub-data-model/images/deal.png">
</p>

<p align="center">
  <img src="https://yalewkidane.github.io/cityhub-data-model/images/autoidlabs.png">
</p>


# NGSI-LD Smart Data Model for CITY HUB


## [1.	ID System](#id-system)

## [2.	Environment Data model](#environment-data-model)

### [2.1.	Air Quality Observation (미세먼지 측정)](#air-quality-observation)

### [2.2.  Weather Observation (날씨 관측)](#weather-observation)

### [2.3.  Odor observation (악취 측정)](#odor-observation)

## [3.	Energy Data Model](#energy-data-model)

### [3.1.	Individual Energy Measurement](#individual-energy-measurement)

### [3.2.	Facility Energy	Usage Measurment](#facility-energy-usage-measurment)

### [3.3.	Building Energy Usage](#building-energy-usage)

### [3.4.	Individual Electricity Measurement](#individual-electricity-measurement)






## ID System 

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

We applied GS1 ID system to each entity.
Please refer to the following document: 
[식별/분류체계 정의서   Version 1.0](https://yalewkidane.github.io/cityhub-data-model/doc/id-system.pdf)


## Environment  Data model [

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

### Air Quality Observation 

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

#### JSON-LD Example

```json
{
    "id": "urn:epc:id:gsrn:950110153.000.7",
    "type": "AirQualityObserved",
    "createdAt":"2020-03-11T20:10:00,000+09:00",
    "modifiedAt":"2020-03-11T20:10:00,000+09:00",
    "dateObserved": {
        "type": "Property",
        "value": "2020-07-15T11:00:00/2020-07-15T12:00:00"
    },
    "location": {
        "type": "Property",
        "value": {
            "type": "Point",
            "coordinates": [127.1293735, 37.4114423]
        },
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "globalLocationNumber": {
       "type": "Property",
       "value": {
         "sgln": "urn:epc:id:sgln:880.969104.100.41390439739010c606"
       }
    },
    "address":{ 
      "type":"Property",
      "value":{ 
         "addressCountry":"KR",
         "addressRegion":"Gyeonggi-do",
         "addressLocality":"Seongnam-si",
         "streetAddress":"8th Seungin-ro",
         "addressTown":"Yatap-dong"
      }
    },  
    "measurementType": {
        "type": "Property",
        "value": "FixedAirQualityMeasurement"
    },
    "co2": {
        "type": "Property",
        "value": 500,
        "unitCode": "59",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "co": {
        "type": "Property",
        "value": 500,
        "unitCode": "59",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "so2": {
        "type": "Property",
        "value": 11,
        "unitCode": "59",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "o3": {
        "type": "Property",
        "value": 0.028,
        "unitCode": "?",
        "observedAt": "2020-06-27T12:00:00Z"
    }, 
    "no2": {
        "type": "Property",
        "value": 69,
        "unitCode": "59",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "khai": {
        "type": "Property",
        "value": 75,
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "pm10": {
        "type": "Property",
        "value": 13,
        "unitCode": "GP",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "pm25": {
        "type": "Property",
        "value": 8,
        "unitCode": "GP",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "temperature": {
        "type": "Property",
        "value": 65.0,
        "unitCode": "CEL",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "humidity": {
        "type": "Property",
        "value": 65.0,
        "unitCode": "P1",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "voc": {
        "type": "Property",
        "value": 0.145,
        "unitCode": "GP",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "noise": {
        "type": "Property",
        "value": 43.0,
        "unitCode": "2N",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "height": {
        "type": "Property",
        "value": 4.5,
        "unitCode": "MTR",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "so2Level": {
        "type": "Property",
        "value": 1,
        "observedAt": "2020-06-27T12:00:00Z"
    },   
    "coLevel": {
        "type": "Property",
        "value": 1,
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "co2Level": {
        "type": "Property",
        "value": 1,
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "no2Level": {
        "type": "Property",
        "value": 1,
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "pm10Level": {
        "type": "Property",
        "value": 1,
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "pm25Level": {
        "type": "Property",
        "value": 1,
        "observedAt": "2020-06-27T12:00:00Z"
    },
    " o3Level": {
        "type": "Property",
        "value": 1,
        "observedAt": "2020-06-27T12:00:00Z"
    },
    " khaiLevel": {
        "type": "Property",
        "value": 1,
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "totalIndex": {
        "type": "Property",
        "value": 20,
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "totalCategory": {
        "type": "Property",
        "value": 1,
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/environment/context.jsonld",
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld"
    ]
}


```

#### Key-Value pair

```json
{
    "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/environment/context.jsonld"
    ],
    "id": "urn:epc:id:gsrn:950110153.000.7",
    "type": "AirQualityObserved",
    "dateObserved": "2020-07-15T11:00:00/2020-07-15T12:00:00",
    "location": {
        "type": "Point",
        "coordinates": [
            127.129373,
            37.411442
        ]
    },
    "globalLocationNumber": {
        "sgln": "urn:epc:id:sgln:880.969104.100.41390439739010c606"
    },
    "address": {
        "addressCountry": "KR",
        "addressRegion": "Gyeonggi-do",
        "addressLocality": "Seongnam-si",
        "streetAddress": "8th Seungin-ro",
        "addressTown": "Yatap-dong"
    },
    "measurementType": "FixedAirQualityMeasurement",
    "co2": 500,
    "co": 500,
    "so2": 11,
    "o3": 0.028,
    "no2": 69,
    "khai": 75,
    "pm10": 13,
    "pm25": 8,
    "temperature": 65,
    "humidity": 65,
    "voc": 0.145,
    "noise": 43,
    "height": 4.5,
    "so2Level": 1,
    "coLevel": 1,
    "co2Level": 1,
    "no2Level": 1,
    "pm10Level": 1,
    "pm25Level": 1,
    " o3Level": 1,
    " khaiLevel": 1,
    "totalIndex": 20,
    "totalCategory": 1
}

```

#### JSON-LD Schema

```json
{
    "$schema": "http://json-schema.org/schema#",
    "$schemaVersion": "0.0",
    "$id": "https://cityhub.kr/AirQualityObserved/schema.json",
    "title": " - Air quality observed schema",
    "description": "An observation of air quality conditions at a certain place and time.",
    "type": "object",
    "allOf": [
    {
    "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/GSMA-Commons"
    },
    {
     "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/Location-Commons"
    },
    {
      "properties": {
        "type": {
          "type": "string",
          "enum": ["AirQualityObserved"],
          "description": "NGSI Entity type"
        },
        "globalLocationNumber ": {
          "type": "string",
          "description": "GS1 Global Location Number (GLN/SGLN)"
        },
        "measurementType": {
          "type": "String",
          "enum":["FixedAirQualityMeasurement", "PortableAirQualityMeasurement", "MovableAirQualityMeasurement"],
          "description": "Mobility of the measuring device "
        },
        "co2": {
          "type": "number",
          "minimum": 0,
          "description": "Carbon dioxide"
        },
        "co": {
          "type": "number",
          "minimum": 0,
          "description": "Carbon Monoxide"
        },
        "no2": {
          "type": "number",
          "minimum": 0,
          "description": "Nitrogen dioxide"
        },
        "o3": {
          "type": "number",
          "minimum": 0,
          "description": "ozone"
        },
       "pm10": {
          "type": "number",
          "minimum": 0,
          "description": "Particulate matter 1.0 micrometers or less in diameter"
        },
        "pm25": {
          "type": "number",
          "minimum": 0,
          "description": "Particulate matter 2.5 micrometers or less in diameter"
        },
        "so2": {
          "type": "number",
          "minimum": 0,
          "description": "Sulfur dioxide"
        },
        "voc": {
          "type": "number",
          "minimum": 0,
          "description": "Volatile Organic Compound Concentration (VOC)"
        },
        "noise": {
          "type": "number",
          "minimum": 0,
          "description": "sound level measurement"
        },
        "so2Level": {
          "type": "number",
          "minimum": 0,
          "description": " Level of so2"
        },
        "coLevel": {
          "type": "number",
          "minimum": 0,
          "description": " Level of co"
        },
        "co2Level": {
          "type": "number",
          "minimum": 0,
          "description": " Level of co2"
        },
        "no2Level": {
          "type": "number",
          "minimum": 0,
          "description": " Level of no2"
        },
        "pm10Level": {
          "type": "number",
          "minimum": 0,
          "description": " Level of pm10"
        },
        "pm25Level": {
          "type": "number",
          "minimum": 0,
          "description": "Level of pm25"
        },
        "o3Level": {
          "type": "number",
          "minimum": 0,
          "description": "Level of ozone"
        },
        "khaiLevel": {
          "type": "number",
          "minimum": 0,
          "description": "Level of khai"
        },
        "totalCategory": {
          "type": "number",
          "minimum": 0,
          "description": "Level of total category"
        },
        "totalIndex": {
          "type": "number",
          "minimum": 0,
          "description": "Level of total index"
        }
      }
    }
  ],
  "required": ["id", "type", "dateObserved", "location"]
}

```

### Weather Observation 

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

#### JSON-LD Example

```json
{ 
   "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/environment/context.jsonld",
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld"
    ],
   "id":"urn:epc:id:gsrn:950110153.001.7",
   "type":"WeatherObserved",
   "createdAt":"2020-03-11T20:10:00,000+09:00",
   "modifiedAt":"2020-03-11T20:10:00,000+09:00",
    "dateObserved": {
        "type": "Property",
        "value": "2020-07-15T11:00:00/2020-07-15T12:00:00"
    },
   "location":{ 
      "type":"Property",
      "value":{ 
         "type":"Point",
         "coordinates":[ 
            127.1293735,
            37.4114423
         ]
      },
      "observedAt":"2020-06-27T12:00:00Z"
   },
   "address":{ 
      "type":"Property",
      "value":{ 
         "addressCountry":"KR",
         "addressRegion":"Gyeonggi-do",
         "addressLocality":"Seongnam-si",
         "streetAddress":"8th Seungin-ro",
         "addressTown":"Yatap-dong"
      }
   },
   "globalLocationNumber": {
       "type": "Property",
       "value": {
         "sgln": "urn:epc:id:sgln:880.969104.100.41390439739010c606"
       }
   },
   "height": {
        "type": "Property",
        "value": 4.5,
        "unitCode": "MTR",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "windDirection": {
        "type": "Property",
        "value": 287.1,
        "unitCode": "DD",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "windSpeed": {
        "type": "Property",
        "value": 2.1,
        "unitCode": "MTS",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "humidity": {
        "type": "Property",
        "value": 8,
        "unitCode": "P1",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "atmosphericPressure": {
        "type": "Property",
        "value": 9997.0,
        "unitCode": "A97",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "seaLevelPressure": {
        "type": "Property",
        "value": 9997.0,
        "unitCode": "A97",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "hourlyRainfall": {
        "type": "Property",
        "value": 2.5,
        "unitCode": "?",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "dailyRainfall": {
        "type": "Property",
        "value": 2.5,
        "unitCode": "LD",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "rainType": {
        "type": "Property",
        "value": "false"
    },
    "snowfall": {
        "type": "Property",
        "value": 0.2,
        "unitCode": "?",
        "observedAt": "2020-06-27T12:00:00Z"
    },
    "visibility": {
        "type": "Property",
        "value": 300,
        "unitCode": "?",
        "observedAt": "2020-06-27T12:00:00Z"
    },
   "temperature": {
        "type": "Property",
        "value": 10.2,
        "unitCode": "?",
        "observedAt": "2020-06-27T12:00:00Z"
    },   
    "rainfall": {
        "type": "Property",
        "value": 0.2,
        "unitCode": "?",
        "observedAt": "2020-06-27T12:00:00Z"
    }
}


```
#### Key-Value pair

```json
{
    "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/environment/context.jsonld"
    ],
    "id": "urn:epc:id:gsrn:950110153.001.8",
    "type": "WeatherObserved",
    "dateObserved": "2020-07-15T11:00:00/2020-07-15T12:00:00",
    "location": {
        "type": "Point",
        "coordinates": [
            127.129373,
            37.411442
        ]
    },
    "address": {
        "addressCountry": "KR",
        "addressRegion": "Gyeonggi-do",
        "addressLocality": "Seongnam-si",
        "streetAddress": "8th Seungin-ro",
        "addressTown": "Yatap-dong"
    },
    "globalLocationNumber": {
        "sgln": "urn:epc:id:sgln:880.969104.100.41390439739010c606"
    },
    "height": 4.5,
    "windDirection": 287.1,
    "windSpeed": 2.1,
    "humidity": 8,
    "atmosphericPressure": 9997,
    "seaLevelPressure": 9997,
    "hourlyRainfall": 2.5,
    "dailyRainfall": 2.5,
    "rainType": "false",
    "snowfall": 0.2,
    "visibility": 300,
    "temperature": 10.2,
    "rainfall": 0.2
}


```

#### JSON-LD Schema

```json

{
    "$schema": "http://json-schema.org/schema#",
    "$schemaVersion": "0.0",
    "$id": "https://cityhub.kr/AirQualityObserved/schema.json",
    "title": " - Air quality observed schema",
    "description": "An observation of air quality conditions at a certain place and time.",
    "type": "object",
    "allOf": [
    {
    "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/GSMA-Commons"
    },
    {
     "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/Location-Commons"
    },
    {
      "properties": {
        "type": {
          "type": "string",
          "enum": ["AirQualityObserved"],
          "description": "NGSI Entity type"
        },
        "globalLocationNumber ": {
          "type": "string",
          "description": "GS1 Global Location Number (GLN/SGLN)"
        },
        "windDirection": {
          "type": "number",
          "minimum": 0,
         "maximum": 360,
          "description": "The direction of wind in degree"
        }, 
        "windSpeed": {
          "type": "number",
          "minimum": 0,
          "description": "The speed of wind in m/s"
        }, 
        "atmosphericPressure": {
          "type": "number",
          "minimum": 0,
          "description": " The pressure within the atmosphere of Earth"
        }, 
        "seaLevelPressure": {
          "type": "number",
          "minimum": 0,
          "description": "Standard sea-level pressure"
        }, 
        "rainStatus": {
          "type": "string",
          "enum": ["true", "false"],
          "description": "Precipitation status"
        }, 
        "hourlyRainfall": {
          "type": "number",
          "minimum": 0,
          "description": " Hourly Precipitation Data"
        }, 
        "dailyRainfall": {
          "type": "number",
          "minimum": 0,
          "description": " Daily Precipitation Data""
        }, 
        "rainfall": {
          "type": "number",
          "minimum": 0,
          "description": " Precipitation Data""
        }, 
        "snowfall": {
          "type": "number",
          "minimum": 0,
          "description": " snowfall Data""
        },
        "visibility": {
          "type": "number",
          "minimum": 0,
          "description": " visibility Data""
        },
      }
    }
  ],
  "required": ["id", "type", "dateObserved", "location"]
}


```

### Odor Observation

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

#### JSON-LD Example

```json
{ 
   "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/environment/context.jsonld",
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld"
    ],
   "id":"urn:epc:id:gsrn:950110153.002.7",
   "type":"OdorObserved",
   "createdAt":"2020-03-11T20:10:00,000+09:00",
   "modifiedAt":"2020-03-11T20:10:00,000+09:00",
   "dateObserved": {
        "type": "Property",
        "value": "2020-07-15T11:00:00/2020-07-15T12:00:00"
    },

   "location":{ 
      "type":"Property",
      "value":{ 
         "type":"Point",
         "coordinates":[ 
            127.1293735,
            37.4114423
         ]
      },
      "observedAt":"2020-06-27T12:00:00Z"
   },
   "address":{ 
      "type":"Property",
      "value":{ 
         "addressCountry":"KR",
         "addressRegion":"Gyeonggi-do",
         "addressLocality":"Seongnam-si",
         "streetAddress":"8th Seungin-ro",
         "addressTown":"Yatap-dong"
      }
   },
   "globalLocationNumber": {
       "type": "Property",
       "value": {
         "sgln": "urn:epc:id:sgln:880.969104.100.41390439739010c606"
       }
   },
   "tod": {
        "type": "Property",
        "value": 5,
        "observedAt": "2020-06-27T12:00:00Z"
    },
   "h2s": {
        "type": "Property",
        "value": 100.0,
        "unitCode": "59",
        "observedAt": "2020-06-27T12:00:00Z"
    },
   "nh3": {
        "type": "Property",
        "value": 100.0,
        "unitCode": "59",
        "observedAt": "2020-06-27T12:00:00Z"
    },
   "voc": {
        "type": "Property",
        "value": 100.0,
        "unitCode": "GP",
        "observedAt": "2020-06-27T12:00:00Z"
    },
   "temperature": {
        "type": "Property",
        "value": 25.0,
        "unitCode": "CEL",
        "observedAt": "2020-06-27T12:00:00Z"
    },
   "humidity": {
        "type": "Property",
        "value": 50.0,
        "unitCode": "P1",
        "observedAt": "2020-06-27T12:00:00Z"
    }
}



```
#### Key-Value pair

```json
{
    "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/environment/context.jsonld"
    ],
    "id": "urn:epc:id:gsrn:950110153.002.7",
    "type": "OdorObserved",
    "dateObserved": "2020-07-15T11:00:00/2020-07-15T12:00:00",
    "location": {
        "type": "Point",
        "coordinates": [
            127.129373,
            37.411442
        ]
    },
    "address": {
        "addressCountry": "KR",
        "addressRegion": "Gyeonggi-do",
        "addressLocality": "Seongnam-si",
        "streetAddress": "8th Seungin-ro",
        "addressTown": "Yatap-dong"
    },
    "globalLocationNumber": {
        "sgln": "urn:epc:id:sgln:880.969104.100.41390439739010c606"
    },
    "tod": 5,
    "h2s": 100,
    "nh3": 100,
    "voc": 100,
    "temperature": 25,
    "humidity": 50
}


```

#### JSON-LD Schema

```json
{
    "$schema": "http://json-schema.org/schema#",
    "$schemaVersion": "0.0",
    "$id": "https://cityhub.kr/OdorObserved/schema.json",
    "title": " – Odor Observed schema",
    "description": "An observation of odor conditions at a certain place and time.",
    "type": "object",
    "allOf": [
    {
    "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/GSMA-Commons"
    },
    {
     "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/Location-Commons"
    },
    {
      "properties": {
        "type": {
          "type": "string",
          "enum": ["OdorObserved"],
          "description": "NGSI Entity type"
        },
        "globalLocationNumber ": {
          "type": "string",
          "description": "GS1 Global Location Number (GLN/SGLN)"
        },
        "voc": {
          "type": "number",
          "minimum": 0,
          "description": "Volatile Organic Compound Concentration(unit: ㎍/㎥)"
        }, 
        "nh3": {
          "type": "number",
          "minimum": 0,
          "description": " Ammonia(NH3)"
        },
        "h2s": {
          "type": "number",
          "minimum": 0,
         "description": " Hydrogen Sulfide (H2S)"
        },
        "tod": {
          "type": "number",
          "minimum": 0,
          "description": " The intensity of odor in terms of threshold odor number "
        },
        
      }
    }
  ],
  "required": ["id", "type", "dateObserved", "location"]
}


```

## Energy Data Model	


### Individual Energy Measurement

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

#### JSON-LD Example

```json
{ 
   "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/energy/context.jsonld",
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld"
    ],
   "id":"urn:epc:id:gsrn:950110153.007.7",
   "type":"DeviceEnergyObserved",
   "createdAt":"2020-03-11T20:10:00,000+09:00",
   "modifiedAt":"2020-03-11T20:10:00,000+09:00",
   "dateObserved": {
        "type": "Property",
        "value": "2020-07-15T11:00:00/2020-07-15T12:00:00"
    },

   "location":{ 
      "type":"Property",
      "value":{ 
         "type":"Point",
         "coordinates":[ 
            127.1293735,
            37.4114423
         ]
      },
      "observedAt":"2020-06-27T12:00:00Z"
   },
   "address":{ 
      "type":"Property",
      "value":{ 
         "addressCountry":"KR",
         "addressRegion":"Gyeonggi-do",
         "addressLocality":"Seongnam-si",
         "streetAddress":"8th Seungin-ro",
         "addressTown":"Yatap-dong"
      }
   },
   "globalLocationNumber": {
       "type": "Property",
       "value": {
         "sgln": "urn:epc:id:sgln:880.969104.100.41390439739010c606"
       }
   },
   "ip": {
        "type": "Property",
        "value": "255.255.255.0:502"
   },
   "measurmentSequnce": {
        "type": "Property",
        "value": "255.255.255.0:502"
   },
   "sensorAddress": {
        "type": "Property",
        "value": 1,
        "observedAt":"2020-06-27T12:00:00Z"
   },
   "hourlyTotalEnergy": {
        "type": "Property",
        "value": 1000,
        "unitCode": "JOU"
        "observedAt":"2020-06-27T12:00:00Z"
   },
   "hourlyPeakEnergy": {
        "type": "Property",
        "value": 400,
        "unitCode": "JOU"
        "observedAt":"2020-06-27T12:00:00Z"
   },
   "intervalTotalEnergy": {
        "type": "Property",
        "value": {
         "VAL_0":250,
         "VAL_15":400,
         "VAL_30":200,
         "VAL_45":150
        },
        "minInterval": {
           "type": "Property",
           "value": 15,
           "unitCode": "Minute"
         },
        "observedAt":"2020-06-27T12:00:00Z"
   }
}


```
#### Key-Value pair

```json
{
    "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/energy/context.jsonld"
    ],
    "id": "urn:epc:id:gsrn:950110153.007.7",
    "type": "DeviceEnergyObserved",
    "dateObserved": "2020-07-15T11:00:00/2020-07-15T12:00:00",
    "location": {
        "type": "Point",
        "coordinates": [
            127.129373,
            37.411442
        ]
    },
    "address": {
        "addressCountry": "KR",
        "addressRegion": "Gyeonggi-do",
        "addressLocality": "Seongnam-si",
        "streetAddress": "8th Seungin-ro",
        "addressTown": "Yatap-dong"
    },
    "globalLocationNumber": {
        "sgln": "urn:epc:id:sgln:880.969104.100.41390439739010c606"
    },
    "ip": "255.255.255.0:502",
    "measurmentSequnce": "255.255.255.0:502",
    "sensorAddress": 1,
    "hourlyTotalEnergy": 1000,
    "hourlyPeakEnergy": 400,
    "intervalTotalEnergy": {
        "VAL_0": 250,
        "VAL_15": 400,
        "VAL_30": 200,
        "VAL_45": 150
    }
}


```

#### JSON-LD Schema

```json
{
    "$schema": "http://json-schema.org/schema#",
    "$schemaVersion": "0.0",
    "$id": "https://cityhub.kr/deviceEnergyObserved/schema.json",
    "title": " – Device Energy Observed",
    "description": "An observation of energy at a certain place and time.",
    "type": "object",
    "allOf": [
    {
    "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/GSMA-Commons"
    },
    {
     "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/Location-Commons"
    },
    {
      "properties": {
        "type": {
          "type": "string",
          "enum": ["DeviceEnergyObserved"],
          "description": "NGSI Entity type"
        },
        "globalLocationNumber ": {
          "type": "string",
          "description": "GS1 Global Location Number (GLN/SGLN)"
        }, 
        "ip": {
          "type": "string",
          "description": " IP Address"
        }, 
        "measurmentSequnce": {
          "type": "string",
          "description": " Serial number of the measuring device "
        }, 
        "sensorAddress": {
          "type": "string",
          "description": " sensor Address"
        }, 
        "hourlyTotalEnergy": {
          "type": "number",
          "minimum": 0,
          "description": " Total energy usage in an hour"
        },
        "hourlyPeakEnergy": {
          "type": "number",
          "minimum": 0,
          "description": "The maximum value of energy usage in an hour"

        },
        "intervalTotalEnergy": {
          "type": "JSONObject",
          "minimum": 0,
          "description": " The energy usage in an hour divide with intervals"
        },
        
      }
    }
  ],
  "required": ["id", "type", "dateObserved", "location"]
}


```

### Facility Energy	Usage Measurment

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

#### JSON-LD Example

```json
{ 
   "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/energy/context.jsonld",
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld"
    ],
   "id":"urn:epc:id:gsrn:950110153.008.8",
   "type":"FacilityEnergyObserved",
   "createdAt":"2020-03-11T20:10:00,000+09:00",
   "modifiedAt":"2020-03-11T20:10:00,000+09:00",
   "dateObserved": {
        "type": "Property",
        "value": "2020-07-15T11:00:00/2020-07-15T12:00:00"
    },

   "location":{ 
      "type":"Property",
      "value":{ 
         "type":"Point",
         "coordinates":[ 
            127.1293735,
            37.4114423
         ]
      },
      "observedAt":"2020-06-27T12:00:00Z"
   },
   "address":{ 
      "type":"Property",
      "value":{ 
         "addressCountry":"KR",
         "addressRegion":"Gyeonggi-do",
         "addressLocality":"Seongnam-si",
         "streetAddress":"8th Seungin-ro",
         "addressTown":"Yatap-dong"
      }
   },
   "globalLocationNumber": {
       "type": "Property",
       "value": {
         "sgln": "urn:epc:id:sgln:880969104.100.41390439739010c606"
       }
   },
   "companyID": {
        "type": "Relationship",
        "object": "urn:epc:id:sgln:880969104.100.444"
    },
    "buildingID": {
        "type": "Relationship",
        "object": "urn:epc:id:sgln:880969104.400.443"
    },
    "dischargeFacilityCode": {
        "type": "Property",
        "value": "Building name"
    },
    "energyConsumption": {
        "type": "Property",
        "value": 1000,
        "unitCode": "W",
        "observedAt":"2020-06-27T12:00:00Z"
   },
   "fuelCode": {
        "type": "Property",
        "value": "fuelCode"
    },
   "equipmentName": {
        "type": "Property",
        "value": "equipmentName"
    },
    "orderProcess": {
        "type": "Property",
        "value": "orderProcess"
    },
    "orderLocation": {
        "type": "Property",
        "value": "orderLocation"
    },
    "equipmentCode": {
        "type": "Property",
        "value": "equipmentCode"
    },
    "instrumentCode": {
        "type": "Relationship",
       "object": "urn:epc:id:giai:880969104.100.413"
    },
    "processCode": {
        "type": "Property",
        "value": "processCode"
    }
 }


```
#### Key-Value pair

```json
{
    "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/energy/context.jsonld"
    ],
    "id": "urn:epc:id:gsrn:950110153.008.8",
    "type": "FacilityEnergyObserved",
    "dateObserved": "2020-07-15T11:00:00/2020-07-15T12:00:00",
    "location": {
        "type": "Point",
        "coordinates": [
            127.129373,
            37.411442
        ]
    },
    "address": {
        "addressCountry": "KR",
        "addressRegion": "Gyeonggi-do",
        "addressLocality": "Seongnam-si",
        "streetAddress": "8th Seungin-ro",
        "addressTown": "Yatap-dong"
    },
    "globalLocationNumber": {
        "sgln": "urn:epc:id:sgln:880969104.100.41390439739010c606"
    },
    "companyID": "urn:epc:id:sgln:880969104.100.444",
    "buildingID": "urn:epc:id:sgln:880969104.400.443",
    "dischargeFacilityCode": "Building name",
    "energyConsumption": 1000,
    "fuelCode": "fuelCode",
    "equipmentName": "equipmentName",
    "orderProcess": "orderProcess",
    "orderLocation": "orderLocation",
    "equipmentCode": "equipmentCode",
    "instrumentCode": "urn:epc:id:giai:880969104.100.413",
    "processCode": "processCode"
}


```

#### JSON-LD Schema

```json
{
    "$schema": "http://json-schema.org/schema#",
    "$schemaVersion": "0.0",
    "$id": "https://cityhub.kr/FacilityEnergyObserved/schema.json",
    "title": " – Facility Energy Observed",
    "description": "An observation of energy at a certain place and time.",
    "type": "object",
    "allOf": [
    {
    "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/GSMA-Commons"
    },
    {
     "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/Location-Commons"
    },
    {
      "properties": {
        "type": {
          "type": "string",
          "enum": ["FacilityEnergyObserved "],
          "description": "NGSI Entity type"
        },
        "globalLocationNumber ": {
          "type": "string",
          "description": "GS1 Global Location Number (GLN/SGLN)"
        }, 
        "dischargeFacilityCode": {
          "type": "string",
          "description": " Building Name"
        }, 
        "fuelCode": {
          "type": "string",
          "description": " fuel code "
        }, 
        "equipmentName": {
          "type": "string",
          "description": " Name of the equipment "
        }, 
        "orderProcess": {
          "type": "string",
          "description": " order process"
        },
        "orderLocation": {
          "type": "string",
          "description": "order location"
        },
        "equipmentCode": {
          "type": "string",
          "description": "equipment Code "
        },
        "instrumentCode": {
          "type": "string",
          "description": "instrument code "
        },
        "processCode": {
          "type": " number ",
          "minimum": 0,
          "description": " Process code "
        },
        "companyID": { 
           "$ref": " https://cityhub.kr/common/schema.json#company "
        },
        "buildingID": { 
           "$ref": " https://cityhub.kr/common/schema.json#building "
        } 

      }
    }
  ],
  "required": ["id", "type", "dateObserved", "location"]
}


```

### Building Energy Usage

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

#### JSON-LD Example

```json
{
     "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/energy/context.jsonld",
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld"
    ],
   "id":"urn:epc:id:gsrn:950110153.009.9",
   "type":"BuildingEnergyObserved",
   "createdAt":"2020-06-11T20:10:00,000+09:00",
   "modifiedAt":"2020-06-11T20:10:00,000+09:00",
   "dateObserved": {
        "type": "Property",
        "value": "2020-07-15T11:00:00/2020-07-15T12:00:00"
    },
   "location":{ 
      "type":"Property",
      "value":{ 
         "type":"Point",
         "coordinates":[ 
            127.1293735,
            37.4114423
         ]
      },
      "observedAt":"2020-06-27T12:00:00Z"
   },
   "address":{ 
      "type":"Property",
      "value":{ 
         "addressCountry":"KR",
         "addressRegion":"Gyeonggi-do",
         "addressLocality":"Seongnam-si",
         "streetAddress":"8th Seungin-ro",
         "addressTown":"Yatap-dong"
      }
   },
   "globalLocationNumber": {
       "type": "Property",
       "value": {
         "sgln": "urn:epc:id:sgln:880969104.100.41390439739010c606"
       }
   },

   "siteName": {
        "type": "Property",
        "value": "Building name"
    },
   "totalFloorArea": {
        "type": "Property",
        "value": 100,
        "unitCode": "MTK",
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        }
    },
    "coolingArea": {
        "type": "Property",
        "value": 100,
        "unitCode": "MTK",
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        }
    },
    "manCount": {
        "type": "Property",
        "value": 100,
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        },
        "measurementInterval": {
            "type": "Property",
            "value": 1,
            "unitCode": "MON"
        }
    },
    "floatingManCount": {
        "type": "Property",
        "value": 100,
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        },
        "measurementInterval": {
            "type": "Property",
            "value": 1,
            "unitCode": "MON"
        }
    },
    "groundFloorCount": {
        "type": "Property",
        "value": 100,
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        }
    },
    "basementFloorCount": {
        "type": "Property",
        "value": 100,
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        }
    },
    "completionYear": {
        "type": "Property",
        "value": 100
    },
    "kepcoContractName": {
        "type": "Property",
        "value": "일반용(을) 고압A선택2"
    },
   "kepcoContractCapacity": {
        "type": "Property",
        "value": 3500,
        "unitCode": "KWT",
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        }
    },
    "transformerCapacity": {
        "type": "Property",
        "value": 3500,
        "unitCode": "KWT",
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        }
    },
    "transformerCount": {
        "type": "Property",
        "value": 3500,
        "unitCode": "KWT",
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        }
    },
    "coolingCapatity": {
        "type": "Property",
        "value": 3500,
        "unitCode": "KWT",
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        }
    },
    "heatingCapacity": {
        "type": "Property",
        "value": 4500,
        "unitCode": "KWT",
        "modifiedAt": {
            "type": "Property",
            "value":"2020-03-11T20:10:00,000+09:00"
        }
    },
    "totalElectricAmount": {
        "type": "Property",
        "value": 50,
        "unitCode": "KWT",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "totalWaterAmount": {
        "type": "Property",
        "value": 50,
        "unitCode": "Ton",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "totalGasAmount": {
        "type": "Property",
        "value": 204.1,
        "unitCode": "MJ",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "totalDistrictHeatingAmount": {
        "type": "Property",
        "value": 50,
        "unitCode": "Gcal",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "electricLoad": {
        "type": "Property",
        "value": 50,
        "unitCode": "KW",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "electricPeak": {
        "type": "Property",
        "value": 50,
        "unitCode": "KW",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "heatAndCoolAmount": {
        "type": "Property",
        "value": 50,
        "unitCode": "KWH",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "airConditionAmount": {
        "type": "Property",
        "value": 50,
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "hotWaterAmount": {
        "type": "Property",
        "value": 50,
        "unitCode": "?",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "lightAndHeatingAmount": {
        "type": "Property",
        "value": 50,
        "unitCode": "?",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "transportAmount": {
        "type": "Property",
        "value": 41,
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    },
    "etcAmount": {
        "type": "Property",
        "value": 318,
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementDuration": {
            "type": "Property",
            "value": 1,
            "unitCode": "HR"
        }
    }

}


```
#### Key-Value pair

```json
{
    "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/energy/context.jsonld"
    ],
    "id": "urn:epc:id:gsrn:950110153.009.9",
    "type": "BuildingEnergyObserved",
    "dateObserved": "2020-07-15T11:00:00/2020-07-15T12:00:00",
    "location": {
        "type": "Point",
        "coordinates": [
            127.129373,
            37.411442
        ]
    },
    "address": {
        "addressCountry": "KR",
        "addressRegion": "Gyeonggi-do",
        "addressLocality": "Seongnam-si",
        "streetAddress": "8th Seungin-ro",
        "addressTown": "Yatap-dong"
    },
    "globalLocationNumber": {
        "sgln": "urn:epc:id:sgln:880969104.100.41390439739010c606"
    },
    "siteName": "Building name",
    "totalFloorArea": 100,
    "coolingArea": 100,
    "manCount": 100,
    "floatingManCount": 100,
    "groundFloorCount": 100,
    "basementFloorCount": 100,
    "completionYear": 100,
    "kepcoContractName": "일반용(을) 고압A선택2",
    "kepcoContractCapacity": 3500,
    "transformerCapacity": 3500,
    "transformerCount": 3500,
    "coolingCapatity": 3500,
    "heatingCapacity": 4500,
    "totalElectricAmount": 50,
    "totalWaterAmount": 50,
    "totalGasAmount": 204.1,
    "totalDistrictHeatingAmount": 50,
    "electricLoad": 50,
    "electricPeak": 50,
    "heatAndCoolAmount": 50,
    "airConditionAmount": 50,
    "hotWaterAmount": 50,
    "lightAndHeatingAmount": 50,
    "transportAmount": 41,
    "etcAmount": 318
}


```

#### JSON-LD Schema

```json
{
    "$schema": "http://json-schema.org/schema#",
    "$schemaVersion": "0.0",
    "$id": "https://cityhub.kr/BuildingEnergyObserved/schema.json",
    "title": " – Building Energy Observed",
    "description": "An observation of energy at a certain place and time.",
    "type": "object",
    "allOf": [
    {
    "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/GSMA-Commons"
    },
    {
     "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/Location-Commons"
    },
    {
      "properties": {
        "type": {
          "type": "string",
          "enum": ["BuildingEnergyObserved"],
          "description": "NGSI Entity type"
        },
        "globalLocationNumber ": {
          "type": "string",
          "description": "GS1 Global Location Number (GLN/SGLN)"
        }, 
        "siteName": {
          "type": "string",
          "description": " Site Name"
        }, 
        "totalFloorArea": {
          "type": " number ",
          "minimum": 0,
          "description": " The total area of the floor "
        }, 
        "coolingArea": {
          "type": " number ",
          "minimum": 0,
          "description": " The total cooling area of the floor  "
        }, 
        "manCount": {
          "type": " number ",
          "minimum": 0,
          "description": " The total Number of people   "
        },
        "floatingManCount": {
          "type": " number ",
          "minimum": 0,
          "description": " The total Number of ?? people  "
        },
        "groundFloorCount": {
          "type": " number ",
          "minimum": 0,
          "description": " Number of ground floor "
        },
        "basementFloorCount": {
          "type": " number ",
          "minimum": 0,
          "description": " Number of basement floor"
        },
        "completionYear": {
          "type": " number ",
          "minimum": 0,
          "description": " completion Year"
        },
        "kepcoContractName": {
          "type": "string",
          "description": " kepco Contract Name "
        }, 
        "kepcoContractCapacity": {
          "type": " number ",
          "minimum": 0,
          "description": " kepco Contract Name"
        },
        "transformerCapacity": {
          "type": " number ",
          "minimum": 0,
          "description": " Transformer Capacity"
        },
        "transformerCount": {
          "type": " number ",
          "minimum": 0,
          "description": " Transformer Count"
        },
        "coolingCapatity": {
          "type": " number ",
          "minimum": 0,
          "description": " Cooling Capatity "
        },
        "heatingCapacity": {
          "type": " number ",
          "minimum": 0,
          "description": " heating Capacity "
        },
        "totalElectricAmount": {
          "type": " number ",
          "minimum": 0,
          "description": " total Electric Usage"
        },
        "totalWaterAmount": {
          "type": " number ",
          "minimum": 0,
          "description": " Total Water Amount"
        },
        "totalGasAmount": {
          "type": " number ",
          "minimum": 0,
          "description": " total Gas Amount"
        },
        "totalDistrictHeatingAmount": {
          "type": " number ",
          "minimum": 0,
          "description": " Total District Heating Amount"
        },
        "electricLoad": {
          "type": " number ",
          "minimum": 0,
          "description": " electric Load"
        },
        "electricPeak": {
          "type": " number ",
          "minimum": 0,
          "description": " electric Peak "
        },
        "heatAndCoolAmount": {
          "type": " number ",
          "minimum": 0,
          "description": " heat And Cool Amount "
        },
        "airConditionAmount": {
          "type": " number ",
          "minimum": 0,
          "description": "Air Condition Usage Amount "
        },
        "hotWaterAmount": {
          "type": " number ",
          "minimum": 0,
          "description": " Hot Water Usage Amount"
        },
        "lightAndHeatingAmount": {
          "type": " number ",
          "minimum": 0,
          "description": "Light And Heating Usage Amount"
        },
        "transportAmount": {
          "type": " number ",
          "minimum": 0,
          "description": "Transport usage Amount"
        },
        "etcAmount": {
          "type": " number ",
          "minimum": 0,
          "description": " Other Usage Amount "
        }

      }
    }
  ],
  "required": ["id", "type", "dateObserved", "location"]
}


```

### Individual Electricity Measurement

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

#### JSON-LD Example

```json

{
     "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/energy/context.jsonld",
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld"
    ],
   "id":"urn:epc:id:gsrn:950110153.010.10",
   "type":"ElectricityObserved",
   "createdAt":"2020-06-11T20:10:00,000+09:00",
   "modifiedAt":"2020-06-11T20:10:00,000+09:00",
   "dateObserved": {
        "type": "Property",
        "value": "2020-07-15T11:00:00/2020-07-15T12:00:00"
    },
   "location":{ 
      "type":"Property",
      "value":{ 
         "type":"Point",
         "coordinates":[ 
            127.1293735,
            37.4114423
         ]
      },
      "observedAt":"2020-06-27T12:00:00Z"
   },
   "address":{ 
      "type":"Property",
      "value":{ 
         "addressCountry":"KR",
         "addressRegion":"Gyeonggi-do",
         "addressLocality":"Seongnam-si",
         "streetAddress":"8th Seungin-ro",
         "addressTown":"Yatap-dong"
      }
   },
   "globalLocationNumber": {
       "type": "Property",
       "value": {
         "sgln": "urn:epc:id:sgln:880969104.100.41390439739010c606"
       }
   },
   "instrumentType": {
        "type": "Property",
        "value": "METR_TPCD"
   },
   "totalActivePower": {
        "type": "Property",
        "value": 31700.269531,
        "unitCode": "KWT",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementInterval": {
            "type":"Property",
            "value": 15,
            "unitCode": "D61"
         }
    },
    "totalApparentPower": {
        "type": "Property",
        "value": 36019.089844,
        "unitCode": "D44",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementInterval": {
            "type":"Property",
            "value": 15,
            "unitCode": "D61"
         }
    },
    "totalReactivePower": {
        "type": "Property",
        "value": -7830.332031,
        "unitCode": "D44",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementInterval": {
            "type":"Property",
            "value": 15,
            "unitCode": "D61"
         }
    },
    "expectedTotalReactivePower": {
        "type": "Property",
        "value": -7830.332031,
        "unitCode": "D44",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementInterval": {
            "type":"Property",
            "value": 15,
            "unitCode": "Minute"
         }
    },
    "totalPowerFactor": {
        "type": "Property",
        "value": 0.9,
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementInterval": {
            "type":"Property",
            "value": 15,
            "unitCode": "D61"
         }
    },
   "phaseVoltage": {
        "type": "Property",
        "value": {
            "L1": 234.961304,
            "L2": 234.563477,
            "L3": 235.354034
        },
        "unitCode": "rms",
        "observedAt":"2020-06-27T12:00:00Z",
        "measurementInterval": {
            "type":"Property",
            "value": 15,
            "unitCode": "D61"
         }
    },
    "OTG_RSTN_TYPE": {
        "type": "Property",
        "value": "정복전 구분"
   },
   "numberOfPowerOutage": {
        "type": "Property",
        "value": 11
   }
}

```
#### Key-Value pair

```json
{
    "@context": [
        "https://yalewkidane.github.io/cityhub-data-model/ngsi-ld/energy/context.jsonld"
    ],
    "id": "urn:epc:id:gsrn:950110153.010.10",
    "type": "ElectricityObserved",
    "dateObserved": "2020-07-15T11:00:00/2020-07-15T12:00:00",
    "location": {
        "type": "Point",
        "coordinates": [
            127.129373,
            37.411442
        ]
    },
    "address": {
        "addressCountry": "KR",
        "addressRegion": "Gyeonggi-do",
        "addressLocality": "Seongnam-si",
        "streetAddress": "8th Seungin-ro",
        "addressTown": "Yatap-dong"
    },
    "globalLocationNumber": {
        "sgln": "urn:epc:id:sgln:880969104.100.41390439739010c606"
    },
    "instrumentType": "METR_TPCD",
    "totalActivePower": 31700.269531,
    "totalApparentPower": 36019.089844,
    "totalReactivePower": -7830.332031,
    "expectedTotalReactivePower": -7830.332031,
    "totalPowerFactor": 0.9,
    "phaseVoltage": {
        "L1": 234.961304,
        "L2": 234.563477,
        "L3": 235.354034
    },
    "OTG_RSTN_TYPE": "정복전 구분",
    "numberOfPowerOutage": 11
}


```

#### JSON-LD Schema

```json
{
    "$schema": "http://json-schema.org/schema#",
    "$schemaVersion": "0.0",
    "$id": "https://cityhub.kr/ElectricityObserved/schema.json",
    "title": " –  Electricity Observed",
    "description": "An observation of Electricity at a certain place and time.",
    "type": "object",
    "allOf": [
    {
    "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/GSMA-Commons"
    },
    {
     "$ref": "https://smart-data-models.github.io/data-models/common-schema.json#/definitions/Location-Commons"
    },
    {
      "properties": {
        "type": {
          "type": "string",
          "enum": ["ElectricityObserved"],
          "description": "NGSI Entity type"
        },
        "globalLocationNumber ": {
          "type": "string",
          "description": "GS1 Global Location Number (GLN/SGLN)"
        }, 
        "instrumentType": {
          "type": "string",
          "description": " Instrument Type"
        }, 
        "totalActivePower": {
          "type": "number",
          "description": " Active Power "
        }, 
        "totalApparentPower": {
          "type": "number",
          "description": " Apparent Power "
        }, 
        "totalReactivePower": {
          "type": "number",
          "description": " Reactive Power"
        },
        "expectedTotalReactivePower": {
          "type": "number",
          "description": "Avarage Reactive Power"
        },
        "totalPowerFactor": {
          "type": "string",
          "description": "Power Factor"
        },
        "phaseToPhaseVoltage": {
          "type": "object",
          "properties": {
            "L12": {
              "type": "number",
              "minimum": 0
            },
            "L23": {
              "type": "number",
              "minimum": 0
            },
            "L31": {
              "type": "number",
              "minimum": 0
            }
          },
          "description": " Phase to phase volatage "
        },
        "OTG_RSTN_TYPE": {
          "type": "string"
        },
        "numberOfPowerOutage": {
          "type": " number ",
          "minimum": 0,
          "description": " Number Of Power Outage"
        }

      }
    }
  ],
  "required": ["id", "type", "dateObserved", "location"]
}


```




[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

<p align="center">
  <img src="https://yalewkidane.github.io/cityhub-data-model/images/deal.png">
</p>

<p align="center">
  <img src="https://yalewkidane.github.io/cityhub-data-model/images/autoidlabs.png">
</p>

