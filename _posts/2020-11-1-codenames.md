---
layout: post
title: "Codenames AI"
featured-img: codenames_banner
categories: [Programming]
---

This codenames app is an Android app able to play the role of spymaster in a game of codenames autonomously. It was created as the final project for the Stanford CS238 "Decision Making Under Uncertainty" class and I later turned it into an Android application.

The original bot was a python program that takes user input as for the current game state, and outputs the hint that will give human players the best chance of guessing their words the fastest. To generate hints, it uses a trained neural network model or reads relevant pages off of Wikipedia and creates a graph of all the words in the game and words that connect them. The hints given by this bot have a 60.6% chance of being guessed by humans while hints created by a human have a 67.8% chance.

I created an Android app in Kotlin based on my original Python program to improve the user experience for this tool. In python, I used the word2vec models and Wikipedia entries to find the 1500 most similar words to every word in the game. These are stored in text files and the Android app reads all of these to be able to find connected words. This app is currently available for [download on the Google Play store](https://play.google.com/store/apps/details?id=net.dhvd.codenamesandroidai).

![Playstore Image](/assets/img/posts/codenames/playImage.png)

GitHub Repository for the Python Bot: [https://github.com/T60D/CodenamesAI](https://github.com/T60D/CodenamesAI)

A more detailed overview of how it works:
<iframe width="560" height="315" src="https://www.youtube.com/embed/-TeSpDBu3JE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>