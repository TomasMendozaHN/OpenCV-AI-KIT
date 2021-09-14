
# Detailed instructions can be found here:

https://docs.luxonis.com/en/latest/pages/tutorials/first_steps/#compile-myriadx-blob

But, I summarize them below.

#### Step 1: Install the compiler
pip install --user -U blobconverter

#### Step 2: Go to the folder where your RE-ID OpenVINO .xml and .bin files are located.

#### Step 3: Convert the model
python -m blobconverter --openvino-xml ReId_Cars.xml --openvino-bin ReId_Cars.bin
