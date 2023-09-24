# Kaiburr-Task-2

# 

 Swagger codegen.
Create the same REST API as in task #1, but use [https://editor.swagger.io/](https://editor.swagger.io/) to create your API definition and generate the server code. Choose any java-based server or server framework, that you like. You can either use the online editor or generate the code manually, e.g. using this document: [https://github.com/swagger-api/swagger-codegen/wiki/server-stub-generator-howto](https://github.com/swagger-api/swagger-codegen/wiki/server-stub-generator-howto). Make sure that you can deploy/run the generated code. Once your stub is ready - implement the same functionality as described in task #1, but now in java.
Finally, be sure that you can show how your application responds to requests using postman, curl or any other HTTP client.

## **Prerequisites**

- Docker installed on your system
- Git installed on your system

## **Setup**

### **Step 1: Pull the latest MongoDB image**

```bash
docker pull mongo:latest
```

### **Step 2: Clone the repository**

```bash
git clone https://github.com/SUNIL-RAGHU/kaiburr-Task2.git
```

### **Step 3: Navigate to the repository**

```bash
cd kaiburr-Task2
```

### **Step 4: Build the Docker image for the Spring Boot application**

```bash
docker build -t kaiburr-api .
```

### **Step 5: Open the terminal and navigate to `src/resources`**

```bash
cd src/main/resources
```

### **Step 6: Start the Docker Compose to run MongoDB and the Spring Boot application**

```bash
docker-compose up
```

### ****API Endpoints****

[**http://localhost:9090/swagger-ui/index.html#/**](http://localhost:9090/swagger-ui/index.html#/)

## **`GET /servers/get`**

### **Description**

This endpoint retrieves a list of servers.

### **Request**

- Method: GET
- URL: [http://localhost:9090/swagger-ui/index.html#/server-controller/getAllServers](http://localhost:9090/swagger-ui/index.html#/server-controller/getAllServers)

### 
![GetServerData](https://github.com/shubhankar1962/kaiburr_task2/blob/master/Kaiburr_task2/KaiburrApplication/Task2%20SS/Task2%20getservers%20request.png)

## **`GET /servers/findbyname?name={name}`**

### **Description**

Retrieves a server by its name.

### **Request**

- Method: GET
- URL: [http://localhost:9090/swagger-ui/index.html#/server-controller/findServersByName](http://localhost:9090/swagger-ui/index.html#/server-controller/findServersByName)
- Path Variable: **`name`** (Name of the server)

### GetByName
![GetServerByName](https://github.com/shubhankar1962/kaiburr_task2/blob/master/Kaiburr_task2/KaiburrApplication/Task2%20SS/Task2%20getByname.png)




## **`POST /servers/create`**

### **Description**

This endpoint adds a new server.

### **Request**

- Method: POST
- URL: [http://localhost:9090/swagger-ui/index.html#/server-controller/createServer](http://localhost:9090/swagger-ui/index.html#/server-controller/createServer)
- Body: JSON Object

###
![Postdata]https://github.com/shubhankar1962/kaiburr_task2/blob/master/Kaiburr_task2/KaiburrApplication/Task2%20SS/Task2%20.post%20request.png

### UPDATE Data
![UpdateData](https://github.com/shubhankar1962/kaiburr_task2/blob/master/Kaiburr_task2/KaiburrApplication/Task2%20SS/update_the_record_complete_from_true_to_false.png)


## **`DELETE /servers/{id}`**

### **Description**

This endpoint deletes a server.

### **Request**

- Method: DELETE
- URL: [http://localhost:9090/swagger-ui/index.html#/server-controller/deleteServer](http://localhost:9090/swagger-ui/index.html#/server-controller/deleteServer)
- Path Variable: **`id`** (ID of the server to delete)

### 
![DeleteData](https://github.com/shubhankar1962/kaiburr_task2/blob/master/Kaiburr_task2/KaiburrApplication/Task2%20SS/Task2%20deleteById.png)

## **`GET /servers/findbyname?name={name}`**

### **Description**

Retrieves a server by its name.

### **Request**

- Method: GET
- URL: [http://localhost:9090/swagger-ui/index.html#/server-controller/findServersByName](http://localhost:9090/swagger-ui/index.html#/server-controller/findServersByName)
- Path Variable: **`name`** (Name of the server)

###

<img width="1440" alt="Screenshot 2023-09-14 at 9 10 08 PM" src="https://github.com/SUNIL-RAGHU/kaiburr-Task2/assets/89726488/05a4d317-d860-49c9-9afe-b905ec43ddee">
