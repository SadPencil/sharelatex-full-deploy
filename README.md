# sharelatex-full-deploy
This is the so-called "legacy" way as I'm a podman user rather than docker.

# steps

- Edit the settings in `docker-compose.yml` file, especially the `SHARELATEX_SITE_URL`. 

- If the server is located in Mainland China, modify [sharelatex/Dockerfile] to specify a CTAN mirror. A tuna mirror has been provided as a comment.  

- Start the containers.
  ```bash
  podman-compose up -d 
  ```

- Create admin user.
  https://github.com/overleaf/overleaf/wiki/Creating-and-managing-users
