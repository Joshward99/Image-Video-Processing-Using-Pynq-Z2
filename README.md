![](strathclyde.png)
# Image-Video-Processing-Using-Pynq-Z2
The following repo contains the necessary files needed to build and run and Image and video processing system using the PYNQ-Z2 board the design can take an input from the hdmi port and preform various filter processing on the stream such as , greyscaling, canny-edge detection, Median filtering etc.. 
## File List 
- Video_ip.zip
- Final_Notebook.zip
- Video_Filter_Prj_Sysgen.zip
- PYNQ Assignment.ipynb (Found within Final_Notebook.zip)
- Video_Filter.slx (Found within Video_Filter_Prj_Sysgen.zip)
- VideoFilter.bit (Found within Final_Notebook.zip)
- VideoFilter.tlc (Found within Final_Notebook.zip)
## Using the Files
The files should be used as follows :
- Generate IP Block from Video_Processing.slx using simulink
- use Vivado (2018.3 preferrable) and include IP block in Generated block diagram
- Generate Bitstream from vivado 
- Place genertaed .bit and .tlc files (base_wrapper usally) into network drive mapped to ZYNQ-Z2 (usually 192.168.2.99\xilinx)
- run Video_Processing.ipynb jupyter notebook with hdmi_in and hdmi_out connceted respectively 
### side note
Video_ip contains a pre-generated IP block however it is recommended that a new block is generated first and a projected synthasised incase any changes need to be made in system generator.
## Authors 
- Josh Ward @github/joshward99 
- Paul Brockway @github/SPaulB
- Hussain Khurshid
### Credits
Special thanks to David (@github/dnorthcote) for his "sysgen2pynq Video Template"
