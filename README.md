# Read Me
## About
This is the official GitHub-account of the German Federal Statistical Office. GENESIS-Online is the main database of the Federal Statistical Office and provides results of official statistics in a deeply structured way. All data as well as use of the API are available free of charge. For correct use of license/citation terms see [here](https://www-genesis.destatis.de/datenbank/online/#modal=imprint).

[Registered](https://www-genesis.destatis.de/datenbank/online/#modal=login,register) users have access to a RESTful/JSON webservice interface which can be used to integrate data of GENESIS-Online into automated processes. Each request requires username/e-mail address and password. Instead of identifying with username and password, the web service interface can be used with an individual API token that can be found [here](https://www-genesis.destatis.de/datenbank/online/#modal=web-service-api) after signing in. Token authentication can be used for read only purposes, handling of batch jobs and user credentials requires username/e-mail address and password.

The [textual description](https://www-genesis.destatis.de/datenbank/online/docs/GENESIS-Webservices_Introduction.pdf) (PDF, 899kB, File does not meet accessibility standards) of the RESTful/JSON webservice interface provides detailed information on all services of the web service.

This GitHub-repo provides python and VBA example code for the most common services of the RESTful/JSON webservice interface such as table and cube download. A modest familiarity with programming languages would be helpful. For R-users there is the independently developed [restatis](https://github.com/CorrelAid/restatis) package. Code snippets have run successfully but are provided as is.

## API Developments in July 2025
All examples show POST requests. From July 2025 on the RESTful/JSON webservice interface of GENESIS-Online will no longer respond to GET requests. Also, SOAP/XML services will be retired entirely by this date.

## Contents of this repo
[Python_logincheck](https://github.com/StatistischesBundesamt/GENESIS-Online/blob/main/python_logincheck.ipynb): Check credentials and availability or terminate requests

[Python_tablefile](https://github.com/StatistischesBundesamt/GENESIS-Online/blob/main/python_tablefile.ipynb): Download tables

[Python_cubefile](https://github.com/StatistischesBundesamt/GENESIS-Online/blob/main/python_cubefile.ipynb): Research and download cubes

[VBA_logincheck](https://github.com/StatistischesBundesamt/GENESIS-Online/blob/main/vba_logincheck.ipynb): Check credentials and availability or terminate requests

[VBA_tablefile](https://github.com/StatistischesBundesamt/GENESIS-Online/blob/main/vba_tablefile.ipynb): Download tables

## Filing issues
In case of API downtime or issues of unexpected behaviour as well as for general inquiries about our database, please report them directly to our [contact form](https://www.destatis.de/DE/Service/Kontakt/Genesis/Servicekontakt-GENESIS.html). This is the fastest way to find support. 

File issues here in this repo when provided code is not working or doesn’t solve typical use cases. 

## Other GENESIS Instances
The examples on this account are from the database GENESIS-Online. By changing the base URL as well as the credentials and some parameters, the same services and methods can be used for other databases with GENESIS technology such as the [Census database](https://ergebnisse.zensus2022.de/datenbank/online/#modal=web-service-api) or the [Regionaldatenbank Deutschland](https://www.regionalstatistik.de/genesis/online?Menu=Webservice).
