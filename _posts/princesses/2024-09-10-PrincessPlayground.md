---
layout: post
title: Disney Princess Playground
description: Learn more about your favorite Disney Princesses here
courses: {compsci: {week: 4 }}
type: tangibles
hide: true
---

[\~\~Click here to enter the Princess Zone\~\~]({{site.baseurl}}/princess/home)

<br>

[Brainwrite]({{site.baseurl}}/brainwrite)

<br>

![Disney Princess banner]({{site.baseurl}}/images/princesses/princesses.jpg)

<!-- adding disney princess poll -->

<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Voting Poll</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        .container {
            width: 300px;
            margin: 50px auto;
            text-align: center;
        }
        button {
            display: block;
            margin: 10px auto;
            padding: 10px 20px;
            background-color: #eb73af;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #ffd9ea;
            color: #f53b8e;
        }
        .results {
            margin-top: 20px;
        }
        .results div {
            margin: 10px 0;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>Vote for Your Favorite Character</h2>
    <button onclick="vote('Mulan')">Mulan</button>
    <button onclick="vote('Moana')">Moana</button>
    <button onclick="vote('Elsa')">Elsa</button>
    <button onclick="vote('Ariel')">Ariel</button>
    <div class="results" id="results">
        <div>Mulan: <span id="mulanVotes">0</span> votes</div>
        <div>Moana: <span id="moanaVotes">0</span> votes</div>
        <div>Elsa: <span id="elsaVotes">0</span> votes</div>
        <div>Ariel: <span id="arielVotes">0</span> votes</div>
    </div>
    <div class="results" id="results">
     <button onclick="clearVotes()">Clear Votes</button>
     </div>
</div>

<script>
    // Initialize votes from local storage or set defaults if not available
    let votes = {
        Mulan: localStorage.getItem('Mulan') ? parseInt(localStorage.getItem('Mulan')) : 0,
        Moana: localStorage.getItem('Moana') ? parseInt(localStorage.getItem('Moana')) : 0,
        Elsa: localStorage.getItem('Elsa') ? parseInt(localStorage.getItem('Elsa')) : 0,
        Ariel: localStorage.getItem('Ariel') ? parseInt(localStorage.getItem('Ariel')) : 0
    };

    // Function to update the displayed vote counts
    function updateVotesDisplay() {
        document.getElementById('mulanVotes').innerText = votes.Mulan;
        document.getElementById('moanaVotes').innerText = votes.Moana;
        document.getElementById('elsaVotes').innerText = votes.Elsa;
        document.getElementById('arielVotes').innerText = votes.Ariel;
    }

    // Call this function to initialize the vote display
    updateVotesDisplay();

    // Function to handle voting
    function vote(character) {
        votes[character]++;
        localStorage.setItem(character, votes[character]); // Save the updated votes to local storage
        updateVotesDisplay(); // Update the displayed votes
    }

    // Function to clear votes and reset local storage
    function clearVotes() {
        votes = { Mulan: 0, Moana: 0, Elsa: 0, Ariel: 0 };
        localStorage.clear(); // Clear all saved votes from local storage
        updateVotesDisplay(); // Reset the displayed votes
    }
</script>
</body>
</html>