# Friend Event Frontend

This is the frontend for the Friend Event application. It connects to an API to display events.

Please run the backend before run the frontend : https://github.com/fredericBui/friendevent_backend

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/friendeventfrontend.git
    ```

## API Endpoints

The frontend connects to the following API endpoints:

- `GET /api/events` - Retrieve a list of events

## Start with Docker
```
docker build . -t friendevent_frontend
docker run --name friendevent_frontend -p 8089:80 friendevent_frontend
```

## Start with K8S
Kubernetes will use the last image push on Dockerhub
```
kubectl apply -f deployment.yaml
kubectl get pods -w
kubectl get services
minikube service friendevent-frontend-service
```

To destroy
```
kubectl delete -f deployment.yaml
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes.

## License

This project is licensed under the MIT License.