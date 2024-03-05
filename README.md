## Demo MongoDB in K8s using Minikube
 Prerequisites: Have installed and configured MINIKUBE.

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

    