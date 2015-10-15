# eea.demo.plone5onrancher

This repository includes orchestration files for automatically deploy a [Plone 5](https://plone.org/) cluster to a [Rancher PaaS server](http://rancher.com/rancher/) via rancher-compose tool (the rancher-compose tool is like a multi-host version of docker-compose).

## Prerequisites

 - On the private or public cloud: you have installed [Rancher](https://github.com/rancher/rancher) with at least two docker hosts.
 - On your pc/laptop: you have installed the rancher-compose tool you find it from the Rancher server after logging in. To enable rancher-compose to launch services in a Rancher instance, you’ll need to set a couple of environment variables or pass them into the rancher-compose command as an option:RANCHER_URL, RANCHER_ACCESS_KEY, and RANCHER_SECRET_KEY. The access key and secret key will be an [API key](http://docs.rancher.com/rancher/configuration/api-keys/):

   ```
   # Set the url that Rancher is on
   $ export RANCHER_URL=http://server_ip:8080/
   # Set the access key, i.e. username
   $ export RANCHER_ACCESS_KEY=<username_of_key>
   # Set the secret key, i.e. password
   $ export RANCHER_SECRET_KEY=<password_of_key>
  ```
 - You are familiar with Docker concepts.

## How to use it

See the screencasts: 

- [Deployment on Rancher PaaS](https://youtu.be/rMRRDICdyDY)
- [Rolling upgrade and rollback on Rancher](https://youtu.be/lhSQpOMJGiQ)

See also the [lightning talks slides](https://docs.google.com/presentation/d/1f7tUMlMJwkFrZ2K3zTPPePmAoKMQ3ssJhoiVsgGxkb4/edit?usp=sharing) from Plone conf 2015

