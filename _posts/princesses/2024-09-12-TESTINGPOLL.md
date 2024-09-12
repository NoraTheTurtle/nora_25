---
layout: post
title: POLL TEST
description: 
courses: {compsci: {week: 4}}
type: hacks
hide: true
---

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
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #45a049;
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
</div>

<script>
    let votes = {
        Mulan: 0,
        Moana: 0,
        Elsa: 0,
        Ariel: 0
    };

    function vote(character) {
        votes[character]++;
        document.getElementById('mulanVotes').innerText = votes.Mulan;
        document.getElementById('moanaVotes').innerText = votes.Moana;
        document.getElementById('elsaVotes').innerText = votes.Elsa;
        document.getElementById('arielVotes').innerText = votes.Ariel;
    }
</script>

</body>
</html>