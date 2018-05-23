This is a OCR project of DD2424 Deep Learning in Data Science, KTH. 

Our project aims at tect detection and recognition of web images. The codes are divided into two parts:Detection and Recognition.
The original data can be downloaded at https://tianchi.aliyun.com/competition/information.htm?spm=5176.100067.5678.2.19eb6a80Ptr3SM&raceId=231651.
The codes of data processing is included in the folder. readfile.py reads the original images and labels, gives the binarized images and their labels which are written in target_label.py. amend_dictionary.py and dictionary.py give the dictionary of converting label seqences to numbers. dictionary.py reads chinese,txt, which includes mostly used 3500 Chinese characters, English alphabet, numbers and some symbols. amend_dictionary.py reads from target_label.py, adding characters in labels, which are not include in chinese.txt.  
In recognition, we use a structure similar to https://github.com/Belval/CRNN, which focuses on latin character recognition. The structure can be briefly described as CNN-LSTM, and CTC Loss is used.
