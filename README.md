# Z-Stack-Endpoints
A JSON file that contains most of the endpoints documented in the Z-Stack Monitor and Test API.pdf from Texas Instruments. There might be some missing or with incorrect values so double check the ones that you plan on using. These endpoints/APIs were pulled directly from the PDF by a parsing script that I created. The script is not super good looking which is why I didn't post it in this repository.


## Format
The format of each entry in the JSON data follows the example below:
```json
{
    "Section": "3.2.1.7",
    "Name": "DATA_RETRIEVE",
    "Description": "Huge AF incoming message data buffer retrieve command.",
    "Request": {
        "CommandType": "SREQ",
        "Fields": {
            "Timestamp": "4",
            "Index": "2",
            "Length": "1"
        }
    },
    "Length": {
        "min": "0x07",
        "max": "0x07"
    },
    "Cmd0": "0x24",
    "Cmd1": "0x12"
},
```
- Values in `Fields` are in bytes
