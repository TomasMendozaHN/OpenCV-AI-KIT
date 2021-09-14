
# Detailed instructions can be found here:

https://docs.luxonis.com/en/latest/pages/tutorials/first_steps/#compile-myriadx-blob

But, I summarize them below.

#### Step 1: Install the compiler
pip install --user -U blobconverter

#### Step 2: Go to the folder where your RE-ID OpenVINO .xml and .bin files are located.

#### Step 3: Convert the model
python -m blobconverter --openvino-xml ReId_Cars.xml --openvino-bin ReId_Cars.bin

#### Step 4: Move your converted file to a new folder
After the conversion is done in step 3, you will see a message that says: Downloading C:\Users\(path to your file). 

So, go to this path, and you will find your ReID_Cars_openvino_(date).blob

## Important!

I have uploaded my ReID blob network to this folder, for your reference. 
