# Mission 6: Mission Reflection

This mission helped me understand how Docker Compose makes deploying cloud applications easier and more organized. Instead of manually typing several Docker commands to create and connect containers, I could describe the application's services in one `docker-compose.yml` file. This makes deployment more consistent, repeatable, and easier to maintain. If the application needs to be deployed again, I can use the same configuration instead of remembering every command.

I also learned that YAML indentation is very important. YAML uses spaces to show the relationships between services, properties, and values. If I use incorrect indentation or press Tab instead of using spaces, Docker Compose may report a configuration error or interpret the file incorrectly. This taught me to check the formatting carefully before deploying an application.

Environment variables are another important part of the configuration. Variables such as `MYSQL_DATABASE`, `MYSQL_USER`, and `MYSQL_PASSWORD` provide the database settings required by the services. The `MYSQL_HOST=database` variable allows Nextcloud to locate the database through the Compose service name. I also learned that real passwords should be protected and should not be published in a public repository.

Deploying Nextcloud with MariaDB made me appreciate how several components can work together to provide a cloud service. Seeing the application become accessible through a browser made the concepts of containers, networking, and deployment more practical. It showed me that cloud infrastructure can be created and managed efficiently when the correct tools and configuration are used.

Since Mission 1, my understanding of Cloud Computing has developed from learning general cloud concepts to understanding how cloud infrastructure can be implemented. I now have a better appreciation of virtualization, containers, storage, networking, and automation. I also understand that deploying an application is only one part of cloud engineering; security, monitoring, maintenance, and reliable data storage are equally important.

Overall, this mission improved my confidence in using Linux commands, Docker Compose, and GitHub. It encouraged me to continue practicing cloud deployment and to apply these skills to more complex projects in the future.
