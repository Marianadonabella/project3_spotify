# Project 3: Song Recommender 

## Introduction

This repository contains a project made during Data Analytics bootcamp, at Ironhack Barcelona (March,2021).
During this week of the bootcamp we've learnt webscrapping, how to work with APIs, and unsupervised machine learning.

## The Project

The project consists on building a song recommender, based on a song inputed by the user.
On my project, I decided to make a special song recommender: it only recommends songs by female singers.
I took this approach because the music industry is ruled by men, and it makes it difficult for women to succeed, and for consumers to find good music perfomed by female that matches their taste. 
More information about it can be found on the presentation material.

## How it works

The project consists basically in two parts:

1) Building and clustering a database using spotify's API: I looked for playlists of different genres containing only female artists and built a database of around 3.000 songs with them. After that, I used unsupervised machine learning to cluster those songs based on their music features, also provided by spotify (danceability, loudness, accousticness,...)

2) Taking input from user and returning a similar song: once the user inputs a song, I "send" it to spotify's API, and it makes me able to get the music features from that song. Then I see in which cluster it would belong, and recommend another song from this same cluster.


## Workflow

The general workflow can be splitted into 5 main steps:

First step: creating workflow and organizing trello
Second step: learning how to work with spotify API
Third step: building database
Fourth step: building the model and the code
Fifth step: refining parameters and testing


## Future improvements

For the recommender to be more assertive, we should have a much bigger database! Since finding playlists only containing female artists can take some time, I'm leaving the database's size increase for a future improvement.
It could also be interesting to test more parameters and cluster sizes, as well as removing some features, to check if the assertiveness of the model improves or not.


## Content

In this repository you'll find:
- Folder "code": notebooks with the coding process. The one with the final and ready to go model is the one called "main"
- Folder "extra materials": presentation document and video with demonstration of the recommender
