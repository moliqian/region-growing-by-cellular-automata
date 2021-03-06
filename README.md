# RegionGrowingAlgorithm

1. This algorithm is used for object segmentation based on user-chosen seed pixels.
2. This [paper](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.59.8092&rep=rep1&type=pdf) describes the method presented in the code.

## Requirements

1. This module needs Python 2.x, [Numpy](http://www.scipy.org/scipylib/download.html), [SciPy](http://www.scipy.org/scipylib/download.html), [datetime](https://docs.python.org/2/library/datetime.html)

## Citations

Please site the work if you are using this.

*Vezhnevets, Vladimir, and Vadim Konouchine. "GrowCut: Interactive multi-label ND image segmentation by cellular automata." proc. of Graphicon. Vol. 1. 2005.* 

## Usage

### General

	$ python rgca.py examples/sample/star-white-clipart.jpg examples/sample/seeds

runs with threshold (`-t`) of 0.5 and with number of iterations (`-i`) of 50 as default

From terminals

	$ python rgca.py examples/sample/star-white-clipart.jpg examples/sample/seeds -t 0.7 -i 75

reads ``examples/sample/star-white-clipart.jpg`` from sample folder with seeds given in an utf-8 encoded file as like ``examples/sample/seeds`` with threshold of 0.7 and number of iterations as 75

Seeds are be of assumed format
	
	n1,n2
	n3,n4
Run
	
	$ python rgca.py -h

for help regarding arguments to be passed
