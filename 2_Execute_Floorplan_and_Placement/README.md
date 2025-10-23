Run the OpenROAD flow
cmd: 
cd flow
make
(if there is issue use the below kind of command
YOSYS_EXE=~/OpenROAD-flow-scripts/tools/yosys/yosys \
OPENROAD_EXE=~/OpenROAD-flow-scripts/tools/OpenROAD/build/bin/openroad \
make)
![make_cmd](./assets/make_cmd.png)

![output_make](./assets/output_make.png)


Launch the graphical user interface (GUI) to visualize the final layout
cmd:  make gui_final

![make_gui_final](./assets/make_gui_final.png)

![make_gui_final2](./assets/make_gui_final2.png)

![Area_gui](./assets/Area_gui.png)

![Area_gui2](./assets/Area_gui2.png)


verify the above steps.
This concludes the floorplan view and placement using the OpenROAD.
