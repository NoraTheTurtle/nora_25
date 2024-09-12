---
layout: post
hide: True
title: Moana
permalink: /princess/moana
---

{% include nav_princess.html %}

### Moana!

<img src="{{site.baseurl}}/images/princesses/moana.png" alt="moana" width="450" height="250">

**Movie**: Moana (2016)
<br>

**Country of Origin**: Polynesia
<br>

**Movie Length**: 1:43

<p><h2>Click here to learn more about moana!</h2></p>
<button><a href="https://princess.disney.com/moana">Click here!!</a></button>

<script>
    var moana_facts = [
    {fact: "Real pigs were used for the voice of Pua", complexity: "O(1)"},
    {fact: "Maui was originally planned to be the protagonist", complexity: "O(1)"},
    {fact: "Moana was Auli'i Cravalho's, the voice of Moana, first acting gig!", complexity: "O(1)"},
    {fact: "You're Welcome was originally Moana's song", complexity: "O(1)"},
    {fact: "Lin-Manuel Miranda wrote a lot of the music for Moana", complexity: "O(1)"},
    {fact: "The name Moana means ocean", complexity: "O(1)"},
];

var randomIndex = Math.floor(Math.random() * moana_facts.length);
var selectedJoke = moana_facts[randomIndex];
console.log("Joke #" + (randomIndex + 1) + ": " + selectedJoke.joke + " (Complexity: " + selectedJoke.complexity + ")");
</script>