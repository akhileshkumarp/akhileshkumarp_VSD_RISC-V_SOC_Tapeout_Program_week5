OpenROAD is an open-source, autonomous physical design flow for digital integrated circuits from RTL to GDSII. It provides a complete toolchain for chip design including synthesis, floorplanning, placement, routing, and verification. 
Official website: [https://openroad.readthedocs.io](https://openroad.readthedocs.io) 
GitHub: [https://github.com/The-OpenROAD-Project](https://github.com/The-OpenROAD-Project) 

OpenROAD installation guide:

step 1 : Clone openroad repo 
cmd : git clone --recursive https://github.com/The-OpenROAD-Project/OpenROAD-flow-scripts
![clone_OpenROAD](./assets/clone_OpenROAD.png)
cmd : cd OpenROAD-flow-scripts
![clone_OpenROAD-flow-scripts](./assets/cd_OpenROAD-flow-scripts.png)

step 2: Run the Setup Script
cmd : sudo ./setup.sh
![run_setup_script](./assets/run_setup1.png)

![run_setup_script end](./assets/run_setup2.png)

step 3: Build OpenROAD
cmd: ./build_openroad.sh --local
(use "./build_openroad.sh --local --threads 1" if you are facing build errors at the end because of memory/resourse issues)

![build cmd](./assets/build_cmd_start.png)

![building stage](./assets/building2.png)


step 4: Verify installation
cmd: 
source ./env.sh
yosys -help  
openroad -help

if yosys is not installed properly then go inside yosys folder within the tools, and run "make" insdie the ./tools/yosys/ folder

![openroad yosys installed](./assets/yosys_openroad_installed.png)

Errors while installations can be debugged/fixed by using the ways mentioned in the document: 
[OpenROAD Error Fixes Guidance](../doc/openroad_error_fixes_guidance_Akhilesh.pdf)

verify the above steps.
This concludes the installation of the OpenROAD.