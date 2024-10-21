# Homework-3
// Require express
const express = require("express");

// app object
const app = express();

// main page
app.get("/", function(req, res) {
    res.send("Welcome to my first Node.js web site.");
});

// contact page
app.get("/contact", function(req, res) {
    res.send("My name is Vasudeva Annam, and you can reach me at 9372610696 & annam02@franklin.email.edu");
});

// bio page
app.get("/bio", function(req, res) {
    res.send("I am Vasudeva Annam, a dedicated student pursuing a degree in Information Technology with a strong interest in cloud computing and IT service management.");
});

// Starting the server
const port = 8002;
app.listen(port, () => {
    console.log(`Server is running at http://localhost:${port}`);
});
