# Crowd Conf
A crowd sourced list of the best tech conferences. Powering a simple discovery UI => [https://crowdconf.org](https://crowdconf.org).

## How To Contribute

Crowd Conf survives off community contributions. If you want to add your event it is simple. Create a patch or a PR to list.json adding your event to the json array.

Any event that is added needs has the following properties which can be added.

| Field       | Type   | Description                                                                                                                                        | Example                                         | Required |
|-------------|--------|----------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------|----------|
| type        | enum   | The type of event that you are adding. Allowed values: ["conference", "workshop"].                                                                 | "conference"                                    | true     |
| name        | string | The name of the event.                                                                                                                             | "my fancy event"                                | true     |
| url         | string | The url to the event site.                                                                                                                         | "http://fancyevents.com"                        | true     |
| description | string | The description of the event.                                                                                                                      | "a truly glorious occasion"                     | true     |
| location    | object | The location of the event. Split into city & country properties.                                                                                   | {"city": "London", "country": "UK" }            | true     |
| date        | object | The start and end date of the event given in the format: MM-DD-YYYY.                                                                               | {"start": "01-4-2018","end": "01-5-2018"}       | true     |
| tags        | array  | Given tags describing themes of the event.                                                                                                         | ["Frontend","UX"]                               | true     |
| price       | object | Pricing information of the event, providing the highest & lowest price of a ticket. Prices should be given as a float rounded to 2 decimal places. | {"currency":"GBP","high": 600.20,"low": 101.21} | true     |

## Inspiration

This project was inspired by:

[https://github.com/asciidisco/web-conferences-2018](https://github.com/asciidisco/web-conferences-2018)
[https://github.com/AndroidStudyGroup/conferences](https://github.com/AndroidStudyGroup/conferences)

