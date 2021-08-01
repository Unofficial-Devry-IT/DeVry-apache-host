#### Commit Activities
![GitHub last commit](https://img.shields.io/github/last-commit/Unofficial-Devry-IT/DeVry-apache-host?label=Last%20Commit)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/Unofficial-Devry-IT/DeVry-apache-host?label=Commit%20Activity)

#### Stats
![GitHub issues](https://img.shields.io/github/issues/Unofficial-Devry-IT/DeVry-apache-host?label=Issues)
![GitHub pull requests](https://img.shields.io/github/issues-pr/Unofficial-Devry-IT/DeVry-apache-host?label=PRs)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Unofficial-Devry-IT/DeVry-apache-host?label=Size)
![GitHub contributors](https://img.shields.io/github/contributors/Unofficial-Devry-IT/DeVry-apache-host)
![GitHub Repo stars](https://img.shields.io/github/stars/Unofficial-Devry-IT/DeVry-apache-host?label=Stars)

# DeVry-services_apache
This is the deployed Apache Server for our [Unofficial DeVry IT Community](https://www.unofficialdevrycom.dev) website.
 
You can join our discord by clicking [here](https://discord.io/unofficial-DevryIT)

Our bot and website are used in an academic setting for students and professors at DeVry University.
Additional information about our custom bot and other projects can be found [here](https://github.com/Unofficial-Devry-IT)

# SSL How to:
By default the container is setup to forward http and https to the container, the SSL certs have to be installed.

They can be saved in the /conf folder as server.key, privkey.pem, and server.crt; the necessary configurations for SSL is already enabled.
I do this using certbot, and manually renaming the files into the /conf directory.

Since certs expire every 90 days, this is done on the dockerhost machine and then copied into the directory. It can be scripted out, however, I choose to do this manually.

Original version of instructions can be found [here](https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-using-lets-encrypt-certificates-with-wordpress)

Compiled directions can be found [here](https://www.traveryates.com/adding-ssl-cert-to-apache-container/)

Updated: 8.1.2021
