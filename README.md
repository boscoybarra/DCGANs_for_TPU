# Experimental repository to train your own database images on a TPUs with a DCGAN

This repository contains material related to Googles Experimental github that you can checkout in full here:'s [Cloud TPUs](https://github.com/tensorflow/tpu). 

### Important: This README is in minus beta and a work in progress. 👨‍💻 Thanks!

### Tutorials

## Steps to convert your own data into tfrecords for TPU

Get files ready from your csv file and save it locally into your machine.

```
gsutil cat gs://${BUCKET}/data/FILE_NAME.csv | head -5 > /tmp/input.csv
cat /tmp/input.csv
```

```
gsutil cat gs://${BUCKET}/data/FILE_NAME.csv  | sed 's/,/ /g' | awk '{print $2}' | sort | uniq > /tmp/labels.txt
cat /tmp/labels.txt
```


### Set Your Data


## Dependencies


### pip


### Conda Environments
