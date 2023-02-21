# Content Based Image Retreival (Search Engine)


## [Demo](https://www.simple-image-search.xyz/)
![](https://mega.nz/file/F8lSCaZD#JDZ-8Fkz0z3RfxR44Bck-peA-RiOFWOxnzVdPcJ2yDw)

## Workflow
![](http://yusukematsui.me/project/sis/img/overview.png)



## Overview
- Simple image-based image search engine using Keras + Flask. You can launch the search engine just by running two python scripts.
- `offline.py`: This script extracts a deep-feature from each database image. Each feature is a 4096D fc6 activation from a VGG16 model with ImageNet pre-trained weights.
- `server.py`: This script runs a web-server. You can send your query image to the server via a Flask web-interface. The server finds similar images to the query by a simple linear scan.
- GPUs are not required.
