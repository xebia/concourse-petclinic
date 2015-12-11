Concourse CI PoC - Spring Pet Clinic
=============

This test is the result of a collaborative effort at [Xebia](http://www.xebia.com) to investigate new and exciting ways to further the CI/CD movement.

1. Use `vagrant up`
2. Download the `fly` cli from [http://192.168.100.4:8080/](http://192.168.100.4:8080/)
3. Copy `vars_sample.yml` to `vars.yml` and edit appropriately to your docker hub credentials and target docker repository/image. 
4. With fly installed persist the `pipeline.yml` in current directory:

      fly c -c pipeline.yml --vars-from vars.yml petclinic
5. Go to the web interface [http://192.168.100.4:8080/](http://192.168.100.4:8080/) and "unpause" the pipeline and execute a build by clicking on the `build` job and pressing the `+` button on the right.
6. Watch magic happen and proceed destruction of your jenkins "pipelines".


