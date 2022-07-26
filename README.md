# UTILS

### Pip upgrade
python -m pip install --upgrade pip

### JSON - Pretty Print
```
import json 

payload = {"role":"engineering","vst_code":"QFE-AUTO-C8DBB0","enrollUsers":[{"email1":"enrol@qantas.com.au"},{"email1":"me@qantas.com.au"},{"email1":"please@qantas.com.au"},{"email1":"e@qantas.com.au"},{"email1":"e@qantas.com.au"}],"workLocation":"Perth","vst_revisionId":"1","vst_lastUpdated":"1657157039945","vst_revisionInfo":"Revision: 07 Jul 2022","user":"JT","username":"JT","id":74,"formName":"DocuNet Access Form","dateSubmitted":"2022-07-08, 02:24:18 UTC","dateSubmittedLocal":"2022-07-08, 12:24:18 UTC+10"},{"role":"engineering","vst_code":"QFE-AUTO-C8DBB0","enrollUsers":[{"email1":"enrol@qantas.com.au"},{"email1":"me@qantas.com.au"},{"email1":"please@qantas.com.au"}

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
```

### Pdf binary content to file
```
def get_pdf(sub_id: int) -> Any:
    
    query = f'?submittedFormId={sub_id}'
    res: Response = api.sendRequest(lookups.EndPoint.FORM_PDF, "GET", query)
    contents = res.content
    with open(f'submitted_form_id_{sub_id}.pdf', 'wb') as f:
        f.write(contents)
    return res.content
```

