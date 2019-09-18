# CASP Express Deploy

Unbound’s Crypto Asset Security Platform (“**CASP**”) provides the advanced technology and the architecture to secure crypto asset transactions. An overview of the CASP solution is found [here](https://www.unboundtech.com/docs/CASP/CASP_User_Guide-HTML/Content/Products/CASP/CASP_Offering_Description/Solution.htm).

CASP can be rapidly deployed using one of these methods:
- [Docker](https://www.docker.com/products/docker-desktop) - Install CASP in a container. This method is intended for POCs.
- [Terraform](https://www.terraform.io/) - Use code to build the CASP infrastructure. This method is intended for production systems.

The rapid installation process is described below. For the full installation process, refer to the [CASP User Guide](https://www.unboundtech.com/docs/CASP/CASP_User_Guide-HTML/Content/Products/CASP/CASP_User_Guide/Installation.htm#Installing-CASP).

## Overview

The CASP implementation is comprised of the following components:

1. **UKC** - Unbound Key Managment servers, including an Entry Point, Partner and Auxiliary server.
2. **PostgreSQL Database** - used by CASP Service.
3. **CASP Services** - including the CASP core service and CASP wallet service.
4. **CASP Bot** - a CASP participant that automatically approves operations.
5. **CASP Web UI** - a web interface used to manage CASP.

Both deployment options install all of the above components. After installation, you can log into the CASP web interface and start using CASP!

<a name="General-Prerequsites"></a>
## General Prerequsites
The following are required before installing CASP. 
1. An Infura access token (for Ethereum ledger access). See [Infura](https://infura.io/register).
   - Register for the Infura site.
   - Create a new project.
   - Copy the access token from the project page.
1. BlockCypher access token (for Bitcoin ledger access). See [BlockCypher](https://accounts.blockcypher.com/signup).
   - Register for the Blockcypher site.
   - After verifying your email, it opens a page that displays the token.
1. Firebase messaging token (to enable push notifications). Contact Unbound for it.

## Installation
After completing the prerequisites, follow the instructions based on the installation type:
- [Docker](./docker)
- [Terraform](./terraform)
