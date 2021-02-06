# Why?

Uses nginx to resolve your docker-automated dev-setup to any domain (like your production domain)

1. So that you have no issues with developing the site locally for licensed themes, which prohibit you from using your license-key on multiple domains
2. So that you can spin up multiple encapsulated wordpress instances with ease
3. So that you an sync your dev-state to wordpress with volumes

# How

Make sure you have docker-compose and docker installed:

1. Resolve the desired host to localhost in your `/etc/hosts` file. For example by running the following:

   ```sh
   echo "127.0.0.1       example.de" >> /etc/hosts
   ```

2. Edit `docker-compose.yaml` to reflect your settings for the db and wordpress

3. Run docker-compose in this folder e.g.:

   ```sh
   docker-compose up
   ```
