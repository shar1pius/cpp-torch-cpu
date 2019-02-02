# C++ inference of a pytorch model on cpu

---
### Application
- Using a resnet model trained on imagenet.

---
## Instructions

- ```pip install -r requirmets.txt```
- Donwload LibTorch cpu & Extract it. [link](https://download.pytorch.org/libtorch/cpu/libtorch-shared-with-deps-latest.zip)
- Clone repository ```git clone https://github.com/Sharwon/cpp-torch-cpu.git```
- Cmake
	``` cd cpp-torch-cpu
	    mkdir build && cd build
	    cmake -DCMAKE_PREFIX_PATH=<full path to libtorch folder> ..
	    make
	```
- Tracing your pytorch model to torch script
	`python model_trace.py`
- mv `.pt` file into models folder
- Test the app ```<app> <model> <image> <label>```
	
---
#### [Colab Notebook : link](https://colab.research.google.com/drive/1A7NTVY4042AD08kaKCOzwKb90FOxmF_M)

---
sample
![](./images/pizza.png ) as ```n07873807 pizza, pizza pie, score: 1.41523```


