## When yoou want to add an attchment in a Outlook email

### First you must to get the all attachments and the content of everyone

{
  "Name": items('Apply_to_each')?['DisplayName'],
  "ContentBytes":  body('Get_attachment_content')
}

