# C++ inference of a pytorch model on cpu

---
### Application
- Using a resnet model trained on imagenet.

---
## Instructions

- ```pip install -r requirmets.txt```
- Donwload LibTorch cpu.
- Clone repository ```git clone```
- Cmake
	``` cd torch_cpp
	    mkdir build && cd build
	    cmake -DCMAKE_PREFIX_PATH=<full path to libtorch folder> ..
	    make
	```
- Tracing your pytorch model to torch script
- Test the app ./example-app ../model.pt ../dog.png ../synset_words.txt
	
---
#### [Colab Notebook : link](https://colab.research.google.com/drive/1A7NTVY4042AD08kaKCOzwKb90FOxmF_M)

---
sample
![](./images/pizza.png ) as ```n07873807 pizza, pizza pie, score: 1.41523```


