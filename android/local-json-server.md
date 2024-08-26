[json-server](https://github.com/typicode/json-server/tree/v0) gives us the ability to supply a fake REST Api endpoint for testing on mobile.

json-server can be installed via NPM:  
    ```npm install -g json-server@0.17.4```

json-server can be ran with:  
    ```json-server --host {IPv4} --watch .\json-server-db.json```

where the {IPv4} address of the machine can be determined by running:  
    ```ipconfig```

an example of a json-server-db.json file can be viewed in this directory:  
    ```example-json-server-db.json```

Retrofit base url should be configured to:  
    ```http://{IPv4}:3000/```

If a field has an "id" with the value 1, it can be returned from a list as such:  
    ```http://{IPv4}:3000/feed/1```

Android manifest must be set up to handle clear text traffic:  
    ```
    <application  
        ...  
        android:usesCleartextTraffic="true">  
     ```  
