### NOTES on setting up the object detecation tensorflow model on Win10 OS

Folder Structure:
```bash
+ model : the root of the project
    + object_detection : the folder of main model scripts
    + slim : tensorflow slim
    - protoc.exe : Protocol Buffers v3.4.0 (link : https://github.com/google/protobuf/releases/tag/v3.4.0)
    
```

install the dependencies
```bash
pip install pillow
pip install lxml
pip install jupyter
pip install matplotlib

```

setup environment 
```bash
protoc object_detection/protos/*.proto --python_out=.
set PYTHONPATH=%PYTHONPATH%;%cd%;%cd%\slim   

```

test the setup 
```bash
python object_detection/builders/model_builder_test.py

```
