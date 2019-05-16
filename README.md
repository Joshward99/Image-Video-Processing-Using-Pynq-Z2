![](strathclyde.png)
# Image-Video-Processing-Using-Pynq-Z2
The following repo contains the necessary files needed to build and run and Image and video processing system using the PYNQ-Z2 board the design can take an input from the hdmi port and preform various filter processing on the stream such as , greyscaling, canny-edge detection, Median filtering etc.. 
## File List 
- Video_ip
- Video_prj
- Video_Processing.ipynb
- Video_processing.slx
- VideoFilter.bit
- VideoFilter.tlc
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
