---
layout: post
title: "Codenames AI"
featured-img: codenames_banner
categories: [Programming]
---

This codenames bot is able to play the role of spymaster in a game of codenames autonomously. It was created as the final project for the Stanford CS238 "Decision Making Under Uncertainty" class.

The bot is a python program that takes user input as for the current game state, and outputs the hint that will give human players the best chance of guessing their words the fastest. To generate hints, it uses a trained neural network model or reads relevant pages off of Wikipedia and creates a graph of all the words in the game and words that connect them. The hints given by this bot have a 60.6% chance of being guessed by humans while hints created by a human have a 67.8% chance.

GitHub Repository: [https://github.com/T60D/CodenamesAI](https://github.com/T60D/CodenamesAI)

A more detailed overview of how it works:
<iframe width="560" height="315" src="https://www.youtube.com/embed/-TeSpDBu3JE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>