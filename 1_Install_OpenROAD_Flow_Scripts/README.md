OpenROAD installation guide:


step 1 : Clone openroad repo 
cmd : git clone --recursive https://github.com/The-OpenROAD-Project/OpenROAD-flow-scripts
cmd : cd OpenROAD-flow-scripts

step 2: Run the Setup Script
cmd : sudo ./setup.sh

step 3: Build OpenROAD
cmd: ./build_openroad.sh --local

step 4: Verify installation
cmd: 
source ./env.sh
yosys -help  
openroad -help

verify the above steps.
This concludes the installation of the OpenROAD.