# Deploy an App at the Edge

Code for Udacity's Intel AI at the edge foundation course: Deploying an app at the edge.
Functionaliy includes deploying an App at the Edge using OpenVino through a command line application.

# Usage

- Use app.py to run each edge application, with the following arguments:

-t: The model type, which should be one of "POSE", "TEXT", or "CAR_META"
-m: The location of the model .xml file
-i: The location of the input image used for testing
-c: A CPU extension file, if applicable. See below for what this is for the workspace. The results of your output will be saved down for viewing in the outputs directory.

- Example function call:

`python app.py -i "images/blue-car.jpg" -t "CAR_META" -m "/home/workspace/models/vehicle-attributes-recognition-barrier-0039.xml" -c "/opt/intel/openvino/deployment_tools/inference_engine/lib/intel64/libcpu_extension_sse4.so"`
