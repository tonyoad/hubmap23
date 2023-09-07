# Kaggle - HuBMAP - Hacking the Human Vasculature

[Offical Page](https://www.kaggle.com/competitions/hubmap-hacking-the-human-vasculature)

## Goal of the Competition

(From official page) 

The goal of this competition is to segment instances of microvascular structures, including capillaries, arterioles, and venules. You'll create a model trained on 2D PAS-stained histology images from healthy human kidney tissue slides.

Your help in automating the segmentation of microvasculature structures will improve researchers' understanding of how the blood vessels are arranged in human tissues.

## Overview

- An instance segmentation compeition. From slides of healthy human kidney tissues, we need to train a model to correctly locate *blood vessels* through masks, and avoid *glomerulus*. 

- The training dataset consists of labelled data from 4 Whole Slide Images (WSI) and unlabelled data from 9 additional WSIs. In labelled data has about 400 carefully labelled images and 1200 sparsely annotated images. In unlabelled data there are about 5400 images.

- Private test set is from another WSI. Public test set is from 2 of the 4 WSI with labelled data. There could be large discrepency between the 2 leaderboards.

## Contents

- Notebook about my attempt for this competition, with result of submissions.

- Transfer learning from pytorch model, experimenting with image augmentation methods, and dilation (a technique largely discussed during the competition)

- (update) New notebook about wrapping code into pytorch-lightning module