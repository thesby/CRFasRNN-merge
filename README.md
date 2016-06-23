# CRFasRNN-merge
This is a repository forked from the latest official caffe-master on Jun 23, 2016. And I merged the latest code of [CRFasRNN](https://github.com/torrvision/crfasrnn) with it. I have simply tested the code, and it worked right. But there is no guarantee for the merge.

If you want to use it, you just need to do as the offical directions. And I really hope that you can add a link to this repository when anything is changed based on it.

#What I have done ?
- add a head file in include/caffe *crfasrnn* to take place of all the old "#include<>".
- copy the *meanfield_iteration.cpp*, and remove the old "#include<>". The same operation was done on *multi_stage_meanfield.cpp*.
- *modified_permutohedral.(hpp,cpp)* are added.
- modified the *caffe.proto* so that MultiStageMeanfield became available.

# How to merge it with other version caffe ?
If you want to do that, you just need to copy the above related files to the correct directories.