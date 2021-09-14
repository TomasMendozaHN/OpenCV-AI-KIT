# Convert YOLO v3 ONNX to OpenVINO! 
## (SAME INSTRUCTIONS AS REID ONNX to OPENVINO)

#### Important: If you have already installed everything, if you have restarted your computer, you must rerun setupvars.bat file.

#### First of all, install OpenVINO con your computer: 
https://docs.openvinotoolkit.org/2021.4/openvino_docs_install_guides_installing_openvino_windows.html#set-the-environment-variables

**Important: You must have Python 3.6-3.8 (3.9 is not supported)

**Important: You must have VisualStudio 19 + CMake (>3.15) installed.

#### Then, install the pre-requisites to make it work with python:
https://docs.openvinotoolkit.org/latest/openvino_docs_MO_DG_prepare_model_Config_Model_Optimizer.html

#### And don't forget to add everything to the PATH:
"C:\Program Files (x86)\Intel\openvino_2021\bin\setupvars.bat"

#### After finishing, open a cmd window and run this:

cd C:\Program Files (x86)\Intel\openvino_2021\deployment_tools\model_optimizer

#### and make sure to put the "YOLO_V3.onnx" file inside the folder above.

python mo.py --input_model=YOLO_V3.onnx --output_dir D: --input_shape (1,3,224,224)

#### this will output 3 files into the root D: drive. Those files are the model in OpenVINO format. 
