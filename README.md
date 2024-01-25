# AccessVibe 

  ![AccessVibe logo](Logo.png)
  
# Introduction 🖋️
AccessVibe is a tech solution that enhances communication for individuals. Designed for inclusivity, it supports individuals with learning disabilities, limited motor skills, visual/hearing impairments.

AccessVibe platform has been created with inclusivity in mind aiming to support individuals, with learning disabilities, limited motor skills and visual impairments.

## Our Features 📑

| ### Speech-to-text	           | ### Text-to-speech         | ### Sign language-to-text |
|--------------------------------|----------------------------|---------------------------|
 This bespoke function utilises<br/> Hello                            |                           |
 verbal input through the user's                            |                           |
 mic to interpret and display      	      	                |                           |
 what was said, in text format.   	      	                |   	      	              |
|   	                               	      	              |   	        	            |
|                                                            |                           |


Data type | Document that string must be |         
--------- | -------
Boolean   | true / false (all lowercase)
Integer   | -2<sup>53</sup>+1 to +2<sup>53</sup>-1 (for consistency with JSON limits on integers [RFC8259](https://datatracker.ietf.org/doc/html/rfc8259))
Float     | [IEEE-754 binary64](https://en.wikipedia.org/wiki/Double-precision_floating-point_format)
String    | (Un)quoted?, max length, legal characters, case-sensitive, multiple delimiter
UUID      | 123e4567-e89b-12d3-a456-426614174000 (no {}s, hyphens, case-insensitive) [RFC4122](https://datatracker.ietf.org/doc/html/rfc4122)
Date/Time (Header) | Sun, 06 Nov 1994 08:49:37 GMT [RFC7231, Section 7.1.1.1](https://datatracker.ietf.org/doc/html/rfc7231#section-7.1.1.1)
Date/Time (Query parameter) | YYYY-MM-DDTHH:mm:ss.sssZ (with at most 3 digits of fractional seconds) [RFC3339](https://datatracker.ietf.org/doc/html/rfc3339)
Byte array | Base-64 encoded, max length
Array      | One of a) a comma-separated list of values (preferred), or b) separate `name=value` parameter instances for each value of the array

Property | Type        | Required | Description
-------- | ----------- | :------: | -----------
`id`     | string      | true     | The unique id of the operation
`status` | string      | true     | enum that includes values "NotStarted", "Running", "Succeeded", "Failed", and "Canceled"
`error`  | ErrorDetail |          | Error object that describes the error when status is "Failed"
`result` | object      |          | Only for POST action-type LRO, the results of the operation when completed successfully
additional<br/>properties | |     | Additional named or dynamic properties of the operation


## Our Purpose 🏹
 _"As the family member of a hard of hearing person, I can understand my relatives better using sign language to text."_ ~ **Allen Humphry**

## My nested checklist
- [x] Task 1
- [ ] Task 2
  - [x] Subtask A
  - [ ] Subtask A
- [x] Task 3
