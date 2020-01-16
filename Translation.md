var c;
var height1;
let e1, e2, e3;

let person;


function setup() {
  createCanvas(600, 400);
  createGraphics(400, 200, WEBGL)
  c= color('hsl(160, 100%, 50%)'); 
  e2 = new Eye(164, 185, 80);
  
  
  
}

function draw() {
  background(0);
  
//HEAD DUDE
 //Top half of head
  strokeWeight(1);
    arc(width/4, height/2, 250, 300, PI, 0.001/PI,           OPEN);
  //Points
  noFill();
 // point(25, height/2);
 // point(55, height/1.3);
 // point(150, height/1.1);
 // point(245, height/1.3);
 // point(275, height/2);
  //bottom of the face
  beginShape();
  curveVertex(25, height/2);
  curveVertex(25, height/2);
  curveVertex(55, height/1.3);
  curveVertex(150, height/1.1);
  curveVertex(245, height/1.3);
  curveVertex(275, height/2);
  curveVertex(275, height/2);
  endShape(OPEN);
  
  strokeWeight(0);
  
  strokeWeight(1);
  fill(0);
  //MOUTH
  
  //TOP
  //top lip center:
  ellipse(width/4,height/1.4,5,5);
  //left cupids
  ellipse(width/4.4,height/1.425,5,5);
  //left corner
 ellipse(width/5.4,height/1.37,5,5);
  //right cupids
 ellipse(width/3.65,height/1.425,5,5);
  //right corner
 ellipse(width/3.1,height/1.37,5,5);
  
  strokeWeight(0);
  
  strokeWeight(1);
  noFill();
  
  beginShape();
 //left corner
  vertex(width/5.4,height/1.37);
  //left cupids
  vertex(width/4.4,height/1.425);
  //center
  vertex(width/4,height/1.4);
  //right cupids
  vertex(width/3.65,height/1.425);
  //right corner
 vertex(width/3.1,height/1.37);
  endShape(OPEN);
  
  
  //MIDDLE
  beginShape();
  curveVertex(width/5.4,height/1.37);
  curveVertex(width/5.4,height/1.37);
 curveVertex(width/4.8,height/1.37);
 curveVertex(width/4.4,height/1.37+random(0,1));
 // curveVertex(width/4.4,mouseY);
 curveVertex(width/3.65,height/1.37+random(0,1));
  //curveVertex(width/3.65,mouseY);
  curveVertex(width/3.4,height/1.37);
   curveVertex(width/3.1,height/1.37);
  curveVertex(width/3.1,height/1.37);
  endShape(OPEN);
  
  beginShape();
 curveVertex(width/5.4,height/1.37);
curveVertex(width/5.4,height/1.37);
 curveVertex(width/4.8,height/1.37);
 curveVertex(width/4.4,height/1.34+random(0,2));
  //curveVertex(width/4.4,mouseX);
 curveVertex(width/3.65,height/1.34+random(0,2));
  //curveVertex(width/3.65,mouseX);
  curveVertex(width/3.4,height/1.37);
   curveVertex(width/3.1,height/1.37);
  curveVertex(width/3.1,height/1.37);
  endShape(OPEN);
  
  
  //BOTTOM
   //TOP
  //top lip center:
  ellipse(width/4,height/1.4,5,5);
  //left cupids
  ellipse(width/4.4,height/1.425,5,5);
  //left corner
 ellipse(width/5.4,height/1.37,5,5);
  //right cupids
 ellipse(width/3.65,height/1.425,5,5);
  //right corner
 ellipse(width/3.1,height/1.37,5,5);
  
  strokeWeight(0);
  
  strokeWeight(1);
  noFill();
  
  beginShape();
 //left corner
  vertex(width/5.4,height/1.37);
  //left cupids
  vertex(width/4.4,height/1.425);
  //center
  vertex(width/4,height/1.4);
  //right cupids
  vertex(width/3.65,height/1.425);
  //right corner
 vertex(width/3.1,height/1.37);
  endShape(OPEN);
  
  beginShape();
  curveVertex(width/5.5,height/1.37);
  curveVertex(width/5.5,height/1.37);
  curveVertex(width/5,height/1.3);
  curveVertex(width/4,height/1.26);
  curveVertex(width/3.27,height/1.3);
  curveVertex(width/3.1,height/1.37);
  curveVertex(width/3.1,height/1.37);
  endShape(OPEN);
  
  ellipse(width/5,height/1.3,5,5);
  ellipse(width/4,height/1.26,5,5);
  ellipse(width/3.27,height/1.3,5,5);
  ellipse(width/3.1,height/1.37,5,5);
  ellipse(width/3.1,height/1.37,5,5);
  
  
  //nostril left
  //leftcorner,left,top inner
  beginShape();
  curveVertex(width/4.75,height/1.7);
  curveVertex(width/4.85,height/1.73);
  curveVertex(width/4.55,height/1.75);
 curveVertex(width/4.3,height/1.7);
 endShape(CLOSE);
  
  //nostril right
  beginShape();
  //right corner
  curveVertex(width/3.4,height/1.7);
  //right
  curveVertex(width/3.345,height/1.73);
  //top
  curveVertex(width/3.545,height/1.75);
  //inner
  curveVertex(width/3.705,height/1.7);
  endShape(CLOSE);
  
  //top of nose
  beginShape();
  //left bottom
  vertex(width/5.22,height/1.7);
  vertex(width/5.22,height/1.74);
  //left mid
  vertex(width/5,height/1.785);
  //left top
  vertex(width/4.45,height/1.8);
  //midle
  vertex(width/4,height/1.7);
  //rigth top
  vertex(width/3.65,height/1.8);
  //right mid
  vertex(width/3.3,height/1.785);
  //right bottom
  vertex(width/3.25,height/1.74);
  vertex(width/3.25,height/1.7);
  endShape(OPEN);
 
   
  //left bottom
  ellipse(width/5.22,height/1.7,5,5);
  //left mid
  ellipse(width/5,height/1.785,5,5);
  //left top
  ellipse(width/4.45,height/1.8,5,5);
  //midle
  ellipse(width/4,height/1.7,5,5);
  //rigth top
  ellipse(width/3.65,height/1.8,5,5);
  //right mid
  ellipse(width/3.3,height/1.785,5,5);
  //right bottom
  ellipse(width/3.25,height/1.7,5,5);
  
  //bridge of nose
  fill(0);
  ellipse(width/4,height/1.99,5,5);
  ellipse(width/4.55,height/1.9,5,5);
  ellipse(width/3.55,height/1.9,5,5);
  //left,mid,right
  
  noFill(0);
   beginShape();
  vertex(width/4.55,height/1.9);
  vertex(width/4,height/1.99);
  vertex(width/3.55,height/1.9);
  endShape(OPEN);
  
  line(width/4,height/1.99,width/4,height/3);
 

//Eye
  e2.update(mouseX, mouseY);
  e2.display();

  
  //right eye
  beginShape();
  //bottom
  vertex(width/2.8,height/2.1);
  //right
  vertex(width/2.5,height/2.4);
  //top
  vertex(width/2.8,height/2.8);
  //left
  vertex(width/3.2,height/2.4);
  endShape(CLOSE);
  
  fill(0);
  ellipse(width/2.8,height/2.1,5,5);
  //right
  ellipse(width/2.5,height/2.4,5,5);
  //top
  ellipse(width/2.8,height/2.8,5,5);
  //left
  ellipse(width/3.2,height/2.4,5,5);
  noFill();
  
  //left eye

  fill(0);
  beginShape();
  vertex(width/6.8,height/2.1);
  vertex(width/9.75,height/2.4);
  vertex(width/6.8,height/2.8);
  vertex(width/5.2,height/2.4);
  endShape(CLOSE);
  noFill();
  
  fill(0);
  rect(73,150,30,30);
  noFill();

  ellipse(width/6.8,height/2.1,5,5);
  //right
  ellipse(width/9.75,height/2.4,5,5);
  //top
  ellipse(width/6.8,height/2.8,5,5);
  //left
  ellipse(width/5.2,height/2.4,5,5);
  
  
 
}

function Eye(tx, ty, ts) {
  this.x = (width/2.8);
  this.y = (height/2.4);
  this.size = 35;
  this.angle = 0;

  this.update = function(mx, my) {
    this.angle = atan2(my - this.y, mx - this.x);
  };
    stroke(c);
  
  this.display = function() {
    push();
    translate(this.x, this.y);
    fill(c);
    ellipse(0, 0, this.size, this.size);
    rotate(this.angle);
    fill(0);
    ellipse((this.size+random(0,1))/ 4, 0, this.size / 2, this.size / 2);
    fill(c);
    ellipse(this.size / 4, 0, this.size / 5, this.size / 5);
    pop();
  };
  
  
  
}
