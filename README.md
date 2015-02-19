# Batch Normalization Layer for Caffe

This implementation of [Batch Normalization](http://arxiv.org/pdf/1502.03167v1.pdf) is based on [MVNLayer](https://github.com/BVLC/caffe/blob/master/src/caffe/layers/mvn_layer.cpp) in Caffe.

To add this layer, you have to modify `common_layers.hpp`, `layer_factory.cpp` and `caffe.proto`. See [Caffe wiki](https://github.com/BVLC/caffe/wiki/Development)

# NOTE

This implementation is very basic which just performs batch normalization computation. Two pieces in [the paper](http://arxiv.org/pdf/1502.03167v1.pdf) are still missing here:
* fixed mean \& variance for inference
* per batch shuffling for thorough randomness
