# WhiteboardToModule

How to Use:

1. Create a whiteboard: Please refer to the examples available in the project. The most important thing is the Snake_Caml case for the workflow names as this will create folders utilizing this naming convention
2. Run the Main (running instead of debug is about 100x faster to utilize)
3. Select your filled out Whiteboardfile. I recommend using the SDD template for all projects.
4. Select the Project folder you want to create your modules in.
5. Select which sheet has the whiteboard in your whiteboard file.
6. Refresh your project to see the new folders/files


## Naming Conventions
### Workflow Name
  Folder_Action_Noun
  The first part of the name will determine the folder for the file to go into. ( Currently, subfolders are not supported. )
  The recommendation after folder is the action being taken and the object the action is being performed on
  
  ### Arguments
   Supported Prefixed:
   * in_
   * out_
   * io_
   
   Supported Delimeters:
   * ;
   * or using alt+enter in excel for newline.
   
   Determining Argument type: (IN PROGRESS, NOT FULLY SUPPORTED)
   * WARNING: do not include special characters in argument types : Including ( ;, <, >, etc)
    utilizng the colong and then type name, the automation will attempt to select that as the data type.
    Example:
    in_name : string
    Will create an in argumeent of type string
    in_date : Datetime
    will create an in argument of type DateTime.
    
    If the data type is invalid, it will default to String.