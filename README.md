# RestRandinRange_POST
Using POST method get a random variable within a specified range

Procedure:
- To run this code you have to create a folder in VS code e.g. RestRandinRange
- Add server.js file to this foler
- Open terminal in VS Code and navigate to your folder e.g. 'cd RestRandinRange'
- Once you are in the project folder, initialize a new Node.js project by running the following command: npm init
- After running npm init, a package.json file will be created in your project folder, which will hold project configuration details and dependencies.
- Now, you can start installing any required Node.js packages for your project. To install the Express.js framework, you can run the following command:
- npm install express body-parser
- This will download and install the Express.js package, adding it to your project's node_modules folder.
- To run your Node.js application from VS Code, open the integrated terminal (if not already open) and use the following command: node server.js
- After running above command in terminal the server will start listening on Port 3000
- Open another terminal and set content-type as application/json
    C:\Users\Kamran\vscodeProjects\RestRandinRange_POST> $headers = @{ 
    >>     "Content-Type" = "application/json"                            
    >> }
- Now invoke the POST method by running below command:
  Invoke-WebRequest -Uri "http://localhost:3000/api/range>> " -Method POST -Headers $headers -Body '{"min": 1, "max": 10}'
- In the above command the range is specified by min & max
