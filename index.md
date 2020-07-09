
<p align="center">
  <img src="https://yalewkidane.github.io/cityhub-data-model/images/cityhubs.png">
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

## Environment  Data model [

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

### Air Quality Observation 

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

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


### Weather Observation 

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

```json


```

### Odor Observation

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

```json


```

## Energy Data Model	

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

```json


```

### Individual Energy Measurement

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

```json


```

### Facility Energy	Usage Measurment

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

```json


```

### Building Energy Usage

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

```json


```

### Individual Electricity Measurement

[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

```json


```



[Go to top](#ngsi-ld-smart-data-model-for-city-hub)

<p align="center">
  <img src="https://yalewkidane.github.io/cityhub-data-model/images/deal.png">
</p>

<p align="center">
  <img src="https://yalewkidane.github.io/cityhub-data-model/images/autoidlabs.png">
</p>



