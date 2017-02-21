make
java svm_toy
java svm_scale -l -1 -u 1 -s range heart.scale > heart.1
java svm_train -s 3 -p 0.1 -t 0 heart.1
java svm_predict -b 1 heart.1 heart.1.model heart.output

