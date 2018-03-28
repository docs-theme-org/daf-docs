
Catalog Manager
============================================================

**Catalog Manager** is the microservice responsible for storing and retrieving metadata associated to the datasets stored in the `DAF <https://github.com/italia/daf/>`__.
It uses a `Docker Compose CKAN  <https://github.com/lorenzoeusepi77/ckanlast>`_ based storage layer as a backend. It is developed following the `OpenApi specification <https://github.com/OAI/OpenAPI-Specification>`_
and contract-first design pattern. 

Every microservice can run as a standalone module using mock data. Not all endpoint can retrieve mock data but all endpoints are described using https://swagger.io/ at localhost:9000/catalog-manager

See `here <../../bigdataplatform/architecture/componentView/index.html>`_ for more details.

.. We recommend to use the local integrated environment with a set of docker described at ......

Local Installation
------------------
- Pre-requisites: JDK 8, SBT, GIT client
- git clone https://github.com/italia/daf
- cd daf/common
- sbt publishLocal
- cd ../catalog_manager
- sbt
- run
- connect to http://localhost:9000/catalog-manager

You should see a swagger UI with all endpoints described.
Nevertheless, the authorization is not required by the UI you should pass at least a Basic authorization token made by an equal user name and password.

To test the endpoints, we suggest to use a tool like `Postman <https://www.getpostman.com/>`_


DAF integration note
--------------------
[TBD]

Endpoints
-------------------
[TBD]

.. This is the recommended installation to work with Daf-dataportal.
