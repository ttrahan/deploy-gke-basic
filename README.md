# Deploy a Node.js application to Google Container Service

![AyeAye](https://github.com/devops-recipes/push-docker-hub/blob/master/public/resources/images/captain.png)

A simple Node JS application with unit tests and coverage reports using mocha
and istanbul. It also does a docker build once CI posses and then pushes the image
to Google Container Registry

## Run CI for this repo on Shippable
* Fork this repo into your local repo
* Login into the [Continuous Integration Service](wwww.shippable.com)
* Create an [integration](http://docs.shippable.com/integrations/imageRegistries/gcr/) on shippable to your google container registry
* All CI configuration is in `shippable.yml`
* Follow these [CI Setup Instructions](http://docs.shippable.com/ci/runFirstBuild/) if you have never used Shippable CI Service
* Update the integrationName in the integration.hub section if you used something other than `shipDH`
* Change the GCR_REPO to point to your repo
* You should be able to run a manual build or webhook build on commit
