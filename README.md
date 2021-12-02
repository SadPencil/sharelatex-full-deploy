# sharelatex-full-deploy
This is the so-called "legacy" way as I'm a podman user rather than docker.

# steps

- Edit the settings in `docker-compose.yml` file, like `SHARELATEX_SITE_URL`. 

- Start the containers.
  ```bash
  podman-compose up -d 
  ```

- Create admin user.
  https://github.com/overleaf/overleaf/wiki/Creating-and-managing-users
