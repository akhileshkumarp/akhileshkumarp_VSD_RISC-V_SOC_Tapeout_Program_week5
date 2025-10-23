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

yosys_openroad_installed.png

verify the above steps.
This concludes the installation of the OpenROAD.