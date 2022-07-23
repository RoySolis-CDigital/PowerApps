## When a user must be save in a sharepointlist column (user or person type) from PowerApps by a Patch or UpdateIf function

### First your must set a variable with the email of the User
Set(UserEmail, User().Email);
### Then in your Patch, UpdateIf function in the user column, save the next object
{
  Claims:"i:0#.f|membership|" & UserEmail,
  Department:"",
  DisplayName:"",
  Email:"",
  JobTitle:"",
  Picture:""
}
