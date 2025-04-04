GitHub Actions Pro Tips
https://www.youtube.com/playlist?list=PLtvmFy4Ed_DL4Vd2uup0ZT6o_HFSaF-yW

actually just some notes about the used actions here...

Check available github actions
https://github.com/actions

To checkout the code use github action:
actions/checkout@v4

Next.js demo site
https://github.com/msusdev-examples/contoso-spaces-next-web-app

To upload the build artifact use github action:
https://github.com/actions/upload-artifact
actions/upload-artifact@v4

To create a github release use action:
https://github.com/actions/create-release
(The create release action seams to need Read and write permissions in settings: Workflow permissions)

An Action to upload a release asset via the GitHub Release API:
https://github.com/actions/upload-release-asset

Build a docker image:
docker build --tag your-user-name/contoso-spaces-web:1.0 .

Run that Docker image:
docker run --detach --publish 5000:80 your-user-name/contoso-spaces-web:1.0

so the built website run from image can be verified locally on:
http://localhost:5000/

Build and push an image to Docker:
https://github.com/docker/build-push-action

To pull the latest docker image use:
docker pull your-user-name/contoso-spaces-web:latest

To run the latest docker image locally use:
docker run --detach --publish 5000:80 your-user-name/contoso-spaces-web:latest

Test it:
http://localhost:5000/



