**<span style="text-decoration:underline;">Exercise</span>:**


**Use the How section above to assist in this exercise**


**Setup**



1. Create a folder on your desktop named ‘UploadForm’
2. Open the folder in Visual Studio Code and create a javascript file. I called mine ‘uploadForm.js’

		**Code**



1. In your .js file, import the http module, the formidable module, and the File System module.
    1. If you haven't installed the formidable npm pack, be sure to use the npm install command to install it.
2. Now, Create a Node.js file that writes an HTML form, with an upload field
    2. Be sure you include your http module here as this will be accessed through your local.
    3. Make your port 3000
3. Include the Formidable module** (if you haven't done so) **to be able to parse the uploaded file once it reaches the server
    4. You’ll need an if statement that checks if the url is currently ending in ‘/fileupload’
    5. If it is, Then parse the incoming form and return a message to the user saying that it has been uploaded
4. Now add the save functionality so that the file is saved to a temporary folder
    6. The path to this directory can be found in the "files" object, passed as the third argument in the parse() method's callback function.
    7. To move the file to the folder of your choice, use the File System module, and then rename the file
