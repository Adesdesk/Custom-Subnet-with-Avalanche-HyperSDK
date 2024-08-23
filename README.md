# Project Title
Custom-Subnet-with-Avalanche-HyperSDK

## Description

This project uses the HyperSDK to demonstrate full control over the rules and functionality of a custom chain, allowing the creation of a custom blockchain that is tailored to a given startup's specific needs. Using the Metacrafters' `tokenvm` repository as starter project, I am able to demonstrate the creation of my custom subnet on which I created, minted and checked my balance of a custom asset.

## Getting Started

### Installing

* To download this program, run the following commands in your teminal, pointing to the location on your computer where the project should be, by running the following command

```
git clone https://github.com/Adesdesk/Custom-Subnet-with-Avalanche-HyperSDK.git
``` 

### Executing program

* Navigate (cd) into this project folder and then into the starter project folder by running the following command

```
cd Custom-Subnet-with-Avalanche-HyperSDK/tokenvm-clone
```

* Run the following command to normalize all the dependencies

```
go mod tidy
```

* Configure the project constants to suit your own requirements
* Go to consts/consts.go and add/edit as applicable.
* Register the Create_Asset and Mint_Assest actions in registry/registry.go
* Run your VM locally

```
Run MODE="run-single" ./scripts/run.sh
Run ./scripts/build.sh
Consult the repository at https://github.com/Metacrafters/tokenvm (also nested within this folder) to see a more detailed guide
```

* Interact with your own HyperChain!
* Use the demos included in the README file of the 'tokenvm-clone' folder
* To close your Local Avalanche Network run the following command 

```
killall avalanche-network-runner
```

## Help

Any advise for common problems or issues.
* Make sure Go is on your path, defined on your terminal, if not you can do so by running export PATH=$PATH:$(go env GOPATH)/bin
If this path doesn’t work, you can also try export PATH=$PATH:/usr/local/go/bin
* If you get a permissions denied error, try running these scripts with the bash command (i.e. bash ./scripts/run.sh)
Load the demo private key included on the project ./build/token-cli key import demo.pk and ./build/token-cli chain import-anr

## Authors

Contributors names and contact info

Name: Adeola David A. 
Email: aadelakun28@gmail.com


## License

This project is licensed under the MIT License - see the LICENSE.md file for details