## When yoou want to add an attchment in a Approval request email

### First you must to get the all attachments and the content of everyone

{
  "Name": items('Apply_to_each')?['DisplayName'],
  "content": {
    "$content-type": body('Get_attachment_content')['$content-type'],
    "$content": body('Get_attachment_content')['$content']
  }
}
