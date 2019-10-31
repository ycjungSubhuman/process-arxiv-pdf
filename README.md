# process-arxiv-pdf

Usually, Arxiv pdf paper files does not contain any metadata and the file names are just numbers. This bash script renames such ArXiv pdf files with more meaningful filenames with title, author, and published date. Also, if available, edits exif metadata.

## Usage

1. Download any ArXiv paper from the site. (i.e. https://arxiv.org/abs/1705.08584)
1. Invoke `process-arxiv-pdf 1705.08584.pdf`
1. The file is renamed to `2017_Li_MMD_GAN:_Towards_Deeper_Understanding_of_Moment_Ma.pdf`. Its metadata can be retrieved with `pdfinfo`

```
$ pdfinfo 2017_Li_MMD_GAN:_Towards_Deeper_Understanding_of_Moment_Ma.pdf
Title:          MMD GAN: Towards Deeper Understanding of Moment Matching Network
Subject:        ArXiv:1705.08584 (2017)
Keywords:
Author:         Li Chun-Liang;Chang Wei-Cheng;Cheng Yu;Yang Yiming;Póczos Barnabás;
Creator:        LaTeX with hyperref package
Producer:       pdfTeX-1.40.17
CreationDate:   Tue Nov 28 11:54:56 2017 KST
ModDate:        Tue Nov 28 11:54:56 2017 KST
Tagged:         no
UserProperties: no
Suspects:       no
Form:           none
JavaScript:     no
Pages:          14
Encrypted:      no
Page size:      612 x 792 pts (letter)
Page rot:       0
File size:      8017745 bytes
Optimized:      no
```
