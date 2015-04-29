# LabComp
Quantizing Quality Values of genomic data to achieve higher compression rates with subsequent lossless compression
Every genomic dataset has the basepair readings along with their corresponding Quality value which is basically a measure of confidence with regard to how sure the sequencing machine is that it has identified the correct basepair. Since only 4 basepairs are possible (A,T,G or C), it makes sense to use Huffman coding to compress the basepairs. There are however a lot more Quality values. Since these values represent confidence measures, it should be tolerable to concede some resolution in return for a higher compression ratio.
As with any lossy compression, there is a tradeoff between compression rate and distortion of data. LabComp is a vector quantization technique which allows you to choose both the vector size and the maximum allowable distortion you would like allow per Quality Value.
