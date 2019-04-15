# Documents

    POST **v1/students/{studentId}/documents**

## Description
List the student's documents, like school reports

## Required Header
* Content-Type: application/json
* Z-Dev-ApiKey: +zorro+
* User-Agent: zorro/1.0
* Z-Auth-Token: token

## Parameters
- **studentId** _(required)_ — your student id obtained with the login

## Response
- **success** — Boolean value.

## Example
**Request**

    https://web.spaggiari.eu/rest/v1/students/{studentId}/documents

**Return** __shortened response__
``` json
 {
   "documents":[
      {
         "hash":"s0m35tr4ng3h4shr1ghth3r3l1k3th1s",
         "desc":"Document title example"
      }
   ],
   "schoolReports":[
      {
         "desc":"Recuperi",
         "confirmLink":"https://web.spaggiari.eu/sol/app/default/pubblicazioni.php?a=RA-LETTURA&desc=Recuperi",
         "viewLink":"https://web.spaggiari.eu/sol/app/default/scrutinio_singolo_recuperi.php?quad=1"
      },
      {
         "desc":"Pagella (Web) Primo Periodo",
         "confirmLink":"https://web.spaggiari.eu/sol\/app/default/pubblicazioni.php?a=RA-LETTURA&desc=Pagella+%28Web%29+Primo+Periodo&sessione=S1",
         "viewLink":"https://web.spaggiari.eu/sol/app/default/genitori_singolo.php?quad=1"
      }
   ]
}
```
