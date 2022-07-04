## Polling App: React + Java Spring Boot (Maven) + MySQL

This example shows how to leverage [Okteto](https://github.com/okteto/okteto) to develop a React + Java Spring Boot (Maven) + MySQL Sample App directly on Okteto Cloud. The Sample App is deployed using a [kustomize](https://github.com/okteto/polling/blob/master/okteto-pipeline.yml). It creates the following components:

- A *React* based **frontend**.
- A Java Spring Boot **api**.
- A [MySQL](https://www.mysql.com/) database.

## Preview

![App Screenshot](screenshot.png)

## Tutorial

- To develop on the **frontend** component:

```
    $ okteto up frontend
      ✓  Development container activated
      ✓  Files synchronized
         Namespace: githubid
         Name:      frontend

    Welcome to your development environment. Happy coding!
    githubid:frontend okteto> yarn install
    githubid:frontend okteto> yarn start
```

- To develop on the **api** component:

```
    $ okteto up api
      ✓  Development container activated
      ✓  Files synchronized
         Namespace: githubid
         Name:      api
         Forward:   5005 -> 5005

    Welcome to your development environment. Happy coding!
    githubid:api okteto> mvn spring-boot:run
```
