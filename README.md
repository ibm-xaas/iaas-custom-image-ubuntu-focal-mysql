# iaas-custom-image-ubuntu-focal-mysql (Work In Progress)
* Note: Just created the repo from template [iaas-custom-image-ubuntu-focal](https://github.com/ibm-xaas/iaas-custom-image-ubuntu-focal)
* Nothing updated yet.


ubuntu 20.04 custom image for ibm cloud
- removed unattended upgrades
- installed docker & docker-compose
- will be installed (not done yet): mysql ... 

## how to test (create a custom image in us-south region)
```
export IBMCLOUD_API_KEY=<YOUR IBMCLOUD API KEY>
docker-compose run packer-ubuntu-focal  ./build_image.sh
```

Due to the limitation of the current packer-plugin-ibm; it's a little difficult to create custom images with multiple regions, that's doable just a little more consideration to be working on. It's good enough for now.
