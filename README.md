# Deploy a Node.js application to Google Container Service

[![Run Status](https://api.shippable.com/projects/58fe2db9baa5e307002d4267/badge?branch=master)](https://app.shippable.com/github/devops-recipes/deploy-gke-basic)[![Coverage Badge](https://api.shippable.com/projects/58fe2db9baa5e307002d4267/coverageBadge?branch=master)](https://app.shippable.com/github/devops-recipes/deploy-gke-basic)

![AyeAye](https://github.com/devops-recipes/push-docker-hub/blob/master/public/resources/images/captain.png)

A simple Node JS application with unit tests and coverage reports using mocha
and istanbul. It also does a docker build once CI passes and then pushes the image
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

## CI Reports on Shippable

### CI Integration View
![CI Integration View](https://github.com/devops-recipes/deploy-gke-basic/blob/master/public/resources/images/gcr-integration.png)

### CI Console Output
![CI Console Output](https://github.com/devops-recipes/deploy-gke-basic/blob/master/public/resources/images/console.jpg)
