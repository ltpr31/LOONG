LOONG is a software to construct auxiliary line based spatial trajectory (ALBST), which faithfully displays spatial relationships of spots along an auxiliary line.

note: LOONG fits Ubuntu 20.04.

Function:

Function "draw_a_loong" provides the interface to construct ALBST.

Command:

/usr/local/LOONG/bin/draw_a_loong  \
--rootPath /path/to/root/path   \
--txtName position.txt  \
--imgName tissue.png \
--outTxtName albst.txt \
--row_std 1 --outImg_height 100  \
--bgImg_height 1000  --bgImg_width 1000

Parameters:

--rootPath: the path saving "position.txt" and "tissue.png", and output folder is to be created here. (Required)
--bgImg_height/width: scaled size of tissue image fitting coordinates of spots. (Not required)
--outTxtName: the file to save ALBST values. (Required)
--txtName: the file saving coordinates of spots. (Required)
--row_std: ALBST will be scaled to 0 to this value. (Not required)
--col_std: Width will be scaled to 0 to this value. If --col_std is not set, Width will be scaled equally with ALBST. (Not required)

Operations:

right-click: draw polygons to select spots involved in ALBST. (Not required)
P key press: draw next polygons. (Not required)
middle-click: save selected spots in polygons. (Not required)
left-click: draw the auxiliary line. (Required)
left double-click: undo all actions. (Not required)
S key press: calculate and save ALBST values. (Required)
