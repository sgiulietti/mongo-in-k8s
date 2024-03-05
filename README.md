## Demo MongoDB in K8s using Minikube
 Prerequisites: Have installed and configured Minikube.

 ### MongoDB

 Step 1: Create a mongodb deployment yaml file.

 Step 2: Create a secret file for reference environment variables.

 Step 3: Convert a plain text to base 64 encoded for use as value of environment variable.
Execute on terminal the following command:

    echo -n ‘someplaintext’ | base64

Copy and use the result as the value of the environment variable.

Step 4: Execute the creation of the secret file.
Navigate on terminal to the folder that contains the file and execute the following command:

    kubectl apply -f secret.yaml

Step 5: Execute the creation of the configuration file.
Navigate on terminal to the folder that contains the file and execute the following command:

    kubectl apply -f confname.yaml

Step 6: Add a service component into the configuration file, then execute the creation of the service component.
Navigate on terminal to the folder that contains the file and execute the following command:

    kubectl apply -f confname.yaml

### Mongo Express

Step 1: Create a mongodb deployment yaml file.

Step 2: Create a configmap file for reference to the database server.

Step 3: Execute the creation of the configmap file and then the configuration of the deployment.
Navigate on terminal to the folder that contains the file and execute the following command:

    kubectl apply -f confirmap.yaml
    kubectl apply -f config.yaml

Step 4: Add a service component into the configuration file, then execute the creation of the service component.
Navigate on terminal to the folder that contains the file and execute the following command:

    kubectl apply -f confname.yaml

Step 5: Make available the UI for mongo express.
Navigate on terminal to the folder that contains the file and execute the following command:

    minikube service servicename        

