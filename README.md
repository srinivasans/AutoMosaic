# AutoMosaic


![AutoMosaic Sample Result](https://raw.githubusercontent.com/srinivasans/AutoMosaic/master/sample.jpg)

Recovery of ripped-up documents is a problem that springs up in Archival study and Investigation science. Efficient and successful joining of torn pieces of papers to reconstruct the original documents is an important and challenging issue which if automated would alleviate the manual effort, which is difficult and time-consuming. This paper focuses on the reconstruction of documents ripped up by hand.

Document reconstruction problems can be solved in two steps, finding an initial set of matching fragment pairs as candidate matches followed by resolving the ambiguity among these candidate matches to reconstruct the original document. Document fragments are represented by their contours and candidate matches are obtained by local curve matching of individual fragments. Local curve matching may result in many ambiguous matches and hence a search technique is required to resolve the ambiguities for global reconstruction.The best-first strategy is one such search technique which selects and merges the best matching pair to form a new fragment. This is repeated until there is only one fragment left which gives the recovered document.

Since document fragments often have similar contour segments in real applications, invalid matching occurs frequently using the local search strategies. Intensive backtracking in such cases makes these local search techniques inefficient. To overcome this, we resort to a global approach to disambiguate the candidate matches. The global consistency approach is based on the fact although some incorrect matches may score higher than the correct one locally, the global score of the correct configuration will be much higher than that of an invalid one. A globally consistent solution is found by exploiting the relationships among all candidate matches.


AutoMosaic is an OpenSource implementation of dynamic programming for reconstruction of torn paper documents. 

Visit https://srinivasans.github.io/AutoMosaic/ for more details. The source code for the implementation is located in https://github.com/raltgz/OpenSoft14
