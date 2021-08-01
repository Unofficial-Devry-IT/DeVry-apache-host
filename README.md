# Devry-services_apache
This is the deployed Apache Server for https://www.unofficialdevrycom.dev website.

You can find our discord at https://discord.io/unofficial-DevryIT

Our bot and website are used in an academic setting for students and professors.

Additional information about our custom bot and other projects can be found at https://github.com/Unofficial-Devry-IT

#SSL Setup:
By default the container is setup to forward http and https to the container, the SSL certs have to be installed.

They can be saved in the /conf folder as server.key, privkey.pem, and server.crt; the necessary configurations for SSL is already enabled.
I do this using certbot, and manually renaming the files into the /conf directory.

Since certs expire every 90 days, this is done on the dockerhost machine and then copied into the directory. It can be scripted out, however, I choose to do this manually.

I used a modified version of the directions found at https://lightsail.aws.amazon.com/ls/docs/en_us/articles/amazon-lightsail-using-lets-encrypt-certificates-with-wordpress

I added directions here https://www.traveryates.com/adding-ssl-cert-to-apache-container/