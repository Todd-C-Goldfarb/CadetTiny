# CadetTiny
Contact: tcgoldfarb@gmail.com

Date: 3/30/2023

This is the Cadet-Tiny model, the first NLP SEQ-2-SEQ model I've ever made, for use on edge devices (such as a raspberry pi). In order to save on computing costs and reduce environmental footprint, I'll be using the pretrained T5-small from Google. It is trained on the SODA dataset, by AllenAI.

Inspired by Cosmo-3B, we will be using the contextual narrative of SODA (n), the perspective/speaker instruction (i), and the dialogue context (c) made up of the previous conversation utterances concatenated with the < TURN > indicator. We will seperate n, i, and c with < SEP >.

(link to the SODA and COSMO paper: https://arxiv.org/pdf/2212.10465.pdf)

(HuggingFace link to the t5-small, the backbone model https://huggingface.co/t5-small)

(HuggingFace link to SODA, the dataset https://huggingface.co/datasets/allenai/soda)

(Special thanks to Hyunwoo Kim for providing personal insight on how to train the model in alignment with how COSMO was trained.)
