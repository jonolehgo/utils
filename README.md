# utils

### JSON pretty print

import json 

payload = {"role":"engineering","vst_code":"QFE-AUTO-C8DBB0","enrollUsers":[{"email1":"enrol@qantas.com.au"},{"email1":"me@qantas.com.au"},{"email1":"please@qantas.com.au"},{"email1":"e@qantas.com.au"},{"email1":"e@qantas.com.au"}],"workLocation":"Perth","vst_revisionId":"1","vst_lastUpdated":"1657157039945","vst_revisionInfo":"Revision: 07 Jul 2022","user":"JT","username":"JT","id":74,"formName":"DocuNet Access Form","dateSubmitted":"2022-07-08, 02:24:18 UTC","dateSubmittedLocal":"2022-07-08, 12:24:18 UTC+10"},{"role":"engineering","vst_code":"QFE-AUTO-C8DBB0","enrollUsers":[{"email1":"enrol@qantas.com.au"},{"email1":"me@qantas.com.au"},{"email1":"please@qantas.com.au"},{"email1":"e@qantas.com.au"}],"workLocation":"Perth","vst_revisionId":"1","vst_lastUpdated":"1657157039945","vst_revisionInfo":"Revision: 07 Jul 2022","user":"JT","username":"JT","id":73,"formName":"DocuNet Access Form","dateSubmitted":"2022-07-08, 02:22:52 UTC","dateSubmittedLocal":"2022-07-08, 12:22:52 UTC+10"},{"role":"engineering","vst_code":"QFE-AUTO-C8DBB0","enrollUsers":[{"email1":"enrol@qantas.com.au"},{"email1":"me@qantas.com.au"},{"email1":"please@qantas.com.au"}],"workLocation":"Perth","vst_revisionId":"1","vst_lastUpdated":"1657157039945","vst_revisionInfo":"Revision: 07 Jul 2022","user":"JT","username":"JT","id":72,"formName":"DocuNet Access Form","dateSubmitted":"2022-07-08, 02:10:30 UTC","dateSubmittedLocal":"2022-07-08, 12:10:30 UTC+10"},{"role":"flightDispatch","vst_code":"QFE-AUTO-C8DBB0","enrollUsers":[{"email1":"test@qantas.com.au"}],"workLocation":"Sydney","vst_revisionId":"1","vst_lastUpdated":"1657157039945","vst_revisionInfo":"Revision: 07 Jul 2022","user":"JT","username":"JT","id":71,"formName":"DocuNet Access Form","dateSubmitted":"2022-07-08, 02:06:46 UTC","dateSubmittedLocal":"2022-07-08, 12:06:46 UTC+10"}

print(json.dumps(payload, indent=4))

{
        "role": "engineering",
        "vst_code": "QFE-AUTO-C8DBB0",
        "enrollUsers": [
            {
                "email1": "enrol@qantas.com.au"
            },
            {
                "email1": "me@qantas.com.au"
            },
            {
                "email1": "please@qantas.com.au"
            },
            {
                "email1": "e@qantas.com.au"
            },
            {
                "email1": "e@qantas.com.au"
            }
        ],
        "workLocation": "Perth",
        "vst_revisionId": "1",
        "vst_lastUpdated": "1657157039945",
        "vst_revisionInfo": "Revision: 07 Jul 2022",
        "user": "JT",
        "username": "JT",
        "id": 74,
        "formName": "DocuNet Access Form",
        "dateSubmitted": "2022-07-08, 02:24:18 UTC",
        "dateSubmittedLocal": "2022-07-08, 12:24:18 UTC+10"
    }
