#  Docker Deployment & Container Lifecycle

##  Nginx Deployment

The Nginx web server was deployed using Docker commands. The process included downloading the Nginx image, creating a container, and checking if the web server was accessible through the browser or terminal.

| Command                                            | Description                                                                                                                 |
| -------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| `docker pull nginx`                                | Retrieves the latest official Nginx image from Docker Hub.                                                                  |
| `docker run -d -p 8080:80 --name web-server nginx` | Creates and starts an Nginx container in the background and connects port 8080 of the computer to port 80 of the container. |
| `curl http://localhost:8080`                       | Sends a request to the local Nginx server to confirm that the deployment is working.                                        |

## Container Management

Docker provides commands for checking, stopping, and deleting containers. These commands were used to demonstrate the basic container lifecycle.

| Command                  | Description                                                                  |
| ------------------------ | ---------------------------------------------------------------------------- |
| `docker ps`              | Displays the Docker containers that are currently running.                   |
| `docker stop web-server` | Stops the Nginx container that is currently running.                         |
| `docker ps -a`           | Shows all Docker containers, including containers that have already stopped. |
| `docker rm web-server`   | Deletes the stopped Nginx container from the system.                         |

## Evidence

Screenshots were captured to document the successful Nginx deployment and the different container management operations. The evidence includes the terminal output showing the running web server and the container lifecycle commands.

**Suggested screenshots:**

* `screenshots/nginx-running.png` – Shows the Nginx container running and the successful HTTP request.
* `screenshots/container-lifecycle.png` – Shows the container being stopped, checked, and removed.
