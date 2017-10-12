# Screensaver-
A p5.js screensaver assignment done with Nick Cook 


var x = 20;
var speed = 0.5;
var r, g, b;

function setup(){
    createCanvas (960,593);
    strokeWeight (2);
    frameRate (10);
    r = random(255);
    g = random(255);
    b = random(255);
}

function draw () {
background(255);
x += speed;
stroke(r, g, b);
fill(r, g, b, 127);

for (var x = 20; x < width; x += 20) {
var mx = mouseX / 10;
var offsetA = random(-mx, mx);
var offsetB = random(-mx, mx);
line(x + offsetA, 0, x - offsetB, 700);
}
    
for (var x = 20; x < width; x += 20) {
var mx = mouseX / 10;
var offsetA = random(-mx, mx);
var offsetB = random(-mx, mx);
line(x + offsetA, 0, x - offsetB, 700);
}
}
   
function mousePressed () {
    r = random(255);
    g = random(255);
    b = random(255);
}
