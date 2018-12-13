let xSize = 400;
let ySize = 400;

let score = 0;

let xDispenser = (xSize/2) - 24.5;
let yDispenser = (ySize/2) - 24.5;
let blok = 7;

let radius = 10;

let credits = false
let startGame = false;
let mainMenu = true;

let player1Wins = false;
let player2Wins = false;

let yart = 100;
let xart = 100;
let b = 10;
let aa = '#ffffff';
let ab = '#d5d5d5';
let ac = '#c8c8c8';
let ad = '#858585';
let ae = '#000000';
let af = '#fda303';
let ag = '#d77c00';
let ah = '#85acae';
let ai = '#699ea0';


function setup(){
  createCanvas(xSize, ySize);
  
  noCursor();
  
  player1 = new player();
  
  player2 = new player0();
  
  mouse1 = new mouse();
  
  dispenser = new art();
  
  ball1 = new ball();
  ball2 = new ball();
  ball3 = new ball();
  ball4 = new ball();
  ball5 = new ball();
  ball6 = new ball();
  
  player1Win = new playerWins();
  player2Win = new player0Wins();

}

function draw() {
  background(80);
      
      
      
      
  if (mainMenu === true) {
  noStroke()   

//credits
  fill('#F7FF03')
	rect(10, 10, 150, 60)
  	textSize(47);
  	fill(0);
  	text('Credits', 11, 56)

//start

  fill('#F7FC3D')
	rect(170, 10, 220, 100) 
	textSize(100);      
	fill(0)   
	text('Start', 170, 100);

//rond bb8
	fill('#F9FC9A')     
	rect(10, 120, 380, 270)
	rect(10, 80, 150, 50)

//bb8 tekening
//hoofd
        {
	fill('#000000')
	rect(xart, yart, b, b)
	fill('#ffffff')
	rect(xart, yart+b, b, b)
	fill('#ffffff')
	rect(xart, yart+2*b, b, b)
	fill('#d5d5d5')
	rect(xart, yart+3*b, b, b)
	fill('#d5d5d5')
	rect(xart, yart+4*b, b, b)
	fill('#d5d5d5')
	rect(xart, yart+5*b, b, b)
	fill('#000000')
	rect(xart, yart+6*b, b, b) 
	fill('#000000')
	rect(xart, yart+7*b, b, b)
	fill('#ffffff')
	rect(xart, yart+8*b, b, b)
	fill('#ffffff')
	rect(xart, yart+9*b, b, b)
	fill('#ffffff')
	rect(xart, yart+10*b, b, b)
	fill('#c8c8c8') 
	rect(xart, yart+11*b, b, b)
	fill('#ffffff')
	rect(xart-b, yart+9*b,b,b)
	fill('#fda303')
	rect(xart-b, yart+10*b,b,b)
	fill('#c8c8c8')
	rect(xart-b, yart+11*b,b,b)
	fill('#c8c8c8')
	rect(xart+b, yart+11*b,b,b)
	fill('#c8c8c8')
	rect(xart+2*b, yart+11*b,b,b)
	fill('#c8c8c8')
	rect(xart+3*b, yart+11*b,b,b)
	fill('#c8c8c8')
	rect(xart+4*b, yart+11*b,b,b)
	fill('#c8c8c8')
	rect(xart+5*b, yart+11*b,b,b)
	fill('#c8c8c8')
	rect(xart+6*b, yart+11*b,b,b)
	fill('#c8c8c8')
	rect(xart+7*b, yart+11*b,b,b)
	fill('#c8c8c8')
	rect(xart+8*b, yart+11*b,b,b)
	fill('#c8c8c8')
	rect(xart+9*b, yart+11*b,b,b)
      fill('#fda303')
	rect(xart+b, yart+10*b,b,b)
	fill('#ffffff')
	rect(xart+2*b, yart+10*b,b,b)
	fill('#fda303')
	rect(xart+3*b, yart+10*b,b,b)
	fill('#fda303')
	rect(xart+4*b, yart+10*b,b,b)
	fill('#ffffff')
	rect(xart+5*b, yart+10*b,b,b)
	fill('#ffffff')
	rect(xart+6*b, yart+10*b,b,b)
	fill('#ffffff')
	rect(xart+7*b, yart+10*b,b,b)
	fill('#d5d5d5')
	rect(xart+8*b, yart+10*b,b,b)
	fill('#ffffff')
	rect(xart+9*b, yart+10*b,b,b) 
	fill('#ffffff')
	rect(xart+1*b, yart+9*b,b,b)
	fill('#ffffff')
	rect(xart+2*b, yart+9*b,b,b)
	fill('#ffffff')
	rect(xart+3*b, yart+9*b,b,b)
  fill('#ffffff')
	rect(xart+4*b, yart+9*b,b,b)
	fill('#ffffff')
	rect(xart+5*b, yart+9*b,b,b)
	fill('#ffffff')
	rect(xart+6*b, yart+9*b,b,b)
	fill('#d5d5d5')
	rect(xart+7*b, yart+9*b,b,b)
	fill('#000000')
	rect(xart+8*b, yart+9*b,b,b)
	fill('#d5d5d5')
	rect(xart+9*b, yart+9*b,b,b)
	fill('#ffffff')
	rect(xart+1*b, yart+8*b,b,b)
	fill('#ffffff')
	rect(xart+2*b, yart+8*b,b,b)
	fill('#ffffff')
	rect(xart+3*b, yart+8*b,b,b)
	fill('#ffffff')
	rect(xart+4*b, yart+8*b,b,b)
	fill('#000000')
	rect(xart+5*b, yart+8*b,b,b)
	fill('#000000')
	rect(xart+6*b, yart+8*b,b,b)
	fill('#ffffff')
	rect(xart+7*b, yart+8*b,b,b)
	fill('#d5d5d5')
	rect(xart+8*b, yart+8*b,b,b)
	fill('#fda303')
	rect(xart+1*b, yart+7*b,b,b)
	fill('#fda303')
	rect(xart+2*b, yart+7*b,b,b)
	fill('#fda303')
	rect(xart+3*b, yart+7*b,b,b)
	fill('#ffffff')
	rect(xart+4*b, yart+7*b,b,b)
	fill('#000000')
	rect(xart+5*b, yart+7*b,b,b)
	fill('#000000')
	rect(xart+6*b, yart+7*b,b,b)
	fill('#ffffff')
	rect(xart+7*b, yart+7*b,b,b)
	fill('#c8c8c8')
	rect(xart+2*b, yart+6*b,b,b)
	fill('#c8c8c8')
	rect(xart+3*b, yart+6*b,b,b)
	fill('#c8c8c8')
	rect(xart+4*b, yart+6*b,b,b)
	fill('#c8c8c8')
	rect(xart+5*b, yart+6*b,b,b)
	fill('#c8c8c8')
	rect(xart+6*b, yart+6*b,b,b)
	fill('#d5d5d5')
	rect(xart+2*b, yart+5*b,b,b)
	fill('#d5d5d5')
	rect(xart+2*b, yart+4*b,b,b)
	fill('#858585')
	rect(xart+1*b, yart+12*b,b,b)
	fill('#858585')
	rect(xart+2*b, yart+12*b,b,b)
	fill('#858585')
	rect(xart+3*b, yart+12*b,b,b)
	fill('#858585')
	rect(xart+4*b, yart+12*b,b,b)
  fill('#858585')
	rect(xart+5*b, yart+12*b,b,b)
	fill('#858585')
	rect(xart+6*b, yart+12*b,b,b)
	fill('#858585')
	rect(xart+7*b, yart+12*b,b,b)


//eerste laag

	fill(ac)
	rect(xart+0*b, yart+13*b,b,b)
	fill(ac)
	rect(xart+1*b, yart+13*b,b,b)
	fill(ac)
	rect(xart+2*b, yart+13*b,b,b)
	fill(ac)
	rect(xart+3*b, yart+13*b,b,b)
	fill(ac)
	rect(xart+4*b, yart+13*b,b,b)
	fill(ac)
	rect(xart+5*b, yart+13*b,b,b)
	fill(ah)
	rect(xart+6*b, yart+13*b,b,b)
	fill(ac)
	rect(xart+7*b, yart+13*b,b,b)
	fill(ac)
	rect(xart+8*b, yart+13*b,b,b)
     
// tweede laag

	fill(af)
	rect(xart-2*b, yart+14*b,b,b)
	fill(ac)
	rect(xart-1*b, yart+14*b,b,b)
  fill(ac)
	rect(xart-0*b, yart+14*b,b,b)
	fill(ac)
	rect(xart+1*b, yart+14*b,b,b)
	fill(ac)
	rect(xart+2*b, yart+14*b,b,b)
	fill(ac)
	rect(xart+3*b, yart+14*b,b,b)
  fill(ac)
	rect(xart+4*b, yart+14*b,b,b)
	fill(ac)
	rect(xart+5*b, yart+14*b,b,b)
	fill(ac)
	rect(xart+6*b, yart+14*b,b,b)
	fill(ac)
	rect(xart+7*b, yart+14*b,b,b)
	fill(aa)
	rect(xart+8*b, yart+14*b,b,b)
	fill(aa)
	rect(xart+9*b, yart+14*b,b,b)
	fill(aa)
	rect(xart+10*b, yart+14*b,b,b)

// derde laag

	fill(af)
	rect(xart-2*b, yart+15*b,b,b)
	fill(ag)
  rect(xart-1*b, yart+15*b,b,b)
	fill(aa)
	rect(xart-0*b, yart+15*b,b,b)
	fill(ac)
	rect(xart+1*b, yart+15*b,b,b)
	fill(ac)
	rect(xart+1*b, yart+15*b,b,b)
	fill(ac)
	rect(xart+2*b, yart+15*b,b,b)
	fill(ac)
	rect(xart+3*b, yart+15*b,b,b)
	fill(ac)
	rect(xart+4*b, yart+15*b,b,b)
	fill(ag)
	rect(xart+5*b, yart+15*b,b,b)
	fill(ag)
	rect(xart+6*b, yart+15*b,b,b)
	fill(ag)
	rect(xart+7*b, yart+15*b,b,b)
	fill(af)
	rect(xart+8*b, yart+15*b,b,b)
	fill(aa)
	rect(xart+9*b, yart+15*b,b,b)
	fill(aa)
	rect(xart+10*b, yart+15*b,b,b)

// vierde laag

	fill(ac)
	rect(xart-3*b, yart+16*b,b,b)
	fill(ag)
	rect(xart-2*b, yart+16*b,b,b)
	fill(ag)
	rect(xart-1*b, yart+16*b,b,b)
	fill(aa)
	rect(xart-0*b, yart+16*b,b,b)
	fill(ai)
	rect(xart+1*b, yart+16*b,b,b)
  fill(ac)
	rect(xart+2*b, yart+16*b,b,b)
	fill(ag)
	rect(xart+3*b, yart+16*b,b,b)
	fill(ag)
	rect(xart+4*b, yart+16*b,b,b)
	fill(ag)
	rect(xart+5*b, yart+16*b,b,b)
	fill(ag)
	rect(xart+6*b, yart+16*b,b,b)
	fill(af)
	rect(xart+7*b, yart+16*b,b,b)
	fill(af)
	rect(xart+8*b, yart+16*b,b,b)
	fill(af)
	rect(xart+9*b, yart+16*b,b,b)
	fill(af)
	rect(xart+10*b, yart+16*b,b,b)
  fill(aa)
	rect(xart+11*b, yart+16*b,b,b)

// vijfde laag

	fill(af)
	rect(xart-3*b, yart+17*b,b,b)
	fill(ag)
	rect(xart-2*b, yart+17*b,b,b)
	fill(ag)
	rect(xart-1*b, yart+17*b,b,b)
	fill(aa)
	rect(xart-0*b, yart+17*b,b,b)
	fill(aa)
	rect(xart+1*b, yart+17*b,b,b)
	fill(aa)
	rect(xart+2*b, yart+17*b,b,b)
	fill(af)
	rect(xart+3*b, yart+17*b,b,b)
	fill(af)
	rect(xart+4*b, yart+17*b,b,b)
	fill(aa)
	rect(xart+5*b, yart+17*b,b,b)
	fill(af)
	rect(xart+6*b, yart+17*b,b,b)
	fill(af)
	rect(xart+7*b, yart+17*b,b,b)
	fill(aa)
	rect(xart+8*b, yart+17*b,b,b)
	fill(af)	
	rect(xart+9*b, yart+17*b,b,b)
	fill(af)
	rect(xart+10*b, yart+17*b,b,b)
	fill(aa)
	rect(xart+11*b, yart+17*b,b,b)
	
// zesde laag

	fill(ah)
	rect(xart-4*b, yart+18*b,b,b)
	fill(af)
	rect(xart-3*b, yart+18*b,b,b)
	fill(ag)
	rect(xart-2*b, yart+18*b,b,b)
	fill(ag)
	rect(xart-1*b, yart+18*b,b,b)
	fill(aa)
	rect(xart-0*b, yart+18*b,b,b)
	fill(aa)
	rect(xart+1*b, yart+18*b,b,b)
	fill(af)
	rect(xart+2*b, yart+18*b,b,b)
	fill(af)
	rect(xart+3*b, yart+18*b,b,b)
	fill(aa)
	rect(xart+4*b, yart+18*b,b,b)
	fill(ai)
	rect(xart+5*b, yart+18*b,b,b)
	fill(aa)
	rect(xart+6*b, yart+18*b,b,b)
	fill(aa)
	rect(xart+7*b, yart+18*b,b,b)
fill(ac)	
rect(xart+8*b, yart+18*b,b,b)
fill(aa)
rect(xart+9*b, yart+18*b,b,b)
fill(af)
rect(xart+10*b, yart+18*b,b,b)
fill(af)
rect(xart+11*b, yart+18*b,b,b)
fill(aa)
rect(xart+12*b, yart+18*b,b,b)

// zevende laag

fill(ac)
rect(xart+-4*b, yart+19*b,b,b)
fill(ag)
rect(xart+-3*b, yart+19*b,b,b)
fill(ag)
rect(xart+-2*b, yart+19*b,b,b)
fill(aa)
rect(xart+-1*b, yart+19*b,b,b)
fill(aa)
rect(xart+-0*b, yart+19*b,b,b)
fill(aa)
rect(xart+1*b, yart+19*b,b,b)
fill(af)
rect(xart+2*b, yart+19*b,b,b)
fill(af)
rect(xart+3*b, yart+19*b,b,b)
fill(af)
rect(xart+4*b, yart+19*b,b,b)
fill(aa)
rect(xart+5*b, yart+19*b,b,b)
fill(ai)
rect(xart+6*b, yart+19*b,b,b)
fill(ac)
rect(xart+7*b, yart+19*b,b,b)
fill(aa)
rect(xart+8*b, yart+19*b,b,b)
fill(af)
rect(xart+9*b, yart+19*b,b,b)
fill(af)
rect(xart+10*b, yart+19*b,b,b)
fill(af)
rect(xart+11*b, yart+19*b,b,b)
fill(aa)
rect(xart+12*b, yart+19*b,b,b)

// achtse laag

fill(af)
rect(xart-4*b, yart+20*b,b,b)
fill(ag)
rect(xart-3*b, yart+20*b,b,b)
fill(ag)
rect(xart-2*b, yart+20*b,b,b)
fill(aa)
rect(xart-1*b, yart+20*b,b,b)
fill(aa)
rect(xart+0*b, yart+20*b,b,b)
fill(aa)
rect(xart+1*b, yart+20*b,b,b)
fill(af)
rect(xart+2*b, yart+20*b,b,b)
fill(af)
rect(xart+3*b, yart+20*b,b,b)
fill(af)
rect(xart+4*b, yart+20*b,b,b)
fill(aa)
rect(xart+5*b, yart+20*b,b,b)
fill(ai)
rect(xart+6*b, yart+20*b,b,b)
fill(ac)
rect(xart+7*b, yart+20*b,b,b)
fill(aa)
rect(xart+8*b, yart+20*b,b,b)
fill(af)
rect(xart+9*b, yart+20*b,b,b)
fill(af)
rect(xart+10*b, yart+20*b,b,b)
fill(af)
rect(xart+11*b, yart+20*b,b,b)
fill(aa)
rect(xart+12*b, yart+20*b,b,b)

// negende laag

fill(af)
rect(xart-4*b, yart+21*b,b,b)
fill(aa)
rect(xart-3*b, yart+21*b,b,b)
fill(aa)
rect(xart-2*b, yart+21*b,b,b)
fill(aa)
rect(xart-1*b, yart+21*b,b,b)
fill(ai)
rect(xart+0*b, yart+21*b,b,b)
fill(aa)
rect(xart+1*b, yart+21*b,b,b)
fill(af)
rect(xart+2*b, yart+21*b,b,b)
fill(af)
rect(xart+3*b, yart+21*b,b,b)
fill(aa)
rect(xart+4*b, yart+21*b,b,b)
fill(ai)
rect(xart+5*b, yart+21*b,b,b)
fill(aa)
rect(xart+6*b, yart+21*b,b,b)
fill(aa)
rect(xart+7*b, yart+21*b,b,b)
fill(ac)
rect(xart+8*b, yart+21*b,b,b)
fill(aa)
rect(xart+9*b, yart+21*b,b,b)
fill(af)
rect(xart+10*b, yart+21*b,b,b)
fill(af)
rect(xart+11*b, yart+21*b,b,b)
fill(aa)
rect(xart+12*b, yart+21*b,b,b)

//tiende laag

fill(ac)
rect(xart-4*b, yart+22*b,b,b)
fill(aa)
rect(xart-3*b, yart+22*b,b,b)
fill(aa)
rect(xart-2*b, yart+22*b,b,b)
fill(aa)
rect(xart-1*b, yart+22*b,b,b)
fill(aa)
rect(xart-0*b, yart+22*b,b,b)
fill(aa)
rect(xart+1*b, yart+22*b,b,b)
fill(aa)
rect(xart+2*b, yart+22*b,b,b)
fill(af)
rect(xart+3*b, yart+22*b,b,b)
fill(af)
rect(xart+4*b, yart+22*b,b,b)
fill(aa)
rect(xart+5*b, yart+22*b,b,b)
fill(af)
rect(xart+6*b, yart+22*b,b,b)
fill(af)
rect(xart+7*b, yart+22*b,b,b)
fill(aa)
rect(xart+8*b, yart+22*b,b,b)
fill(af)
rect(xart+9*b, yart+22*b,b,b)
fill(af)
rect(xart+10*b, yart+22*b,b,b)
fill(aa)
rect(xart+11*b, yart+22*b,b,b)
fill(aa)
rect(xart+12*b, yart+22*b,b,b)

// elfde laag

fill(ah)
rect(yart-3*b, xart+23*b,b,b)
fill(aa)
rect(yart-2*b, xart+23*b,b,b)
fill(aa)
rect(yart-1*b, xart+23*b,b,b)
fill(aa)
rect(yart-0*b, xart+23*b,b,b)
fill(aa)
rect(yart+1*b, xart+23*b,b,b)
fill(aa)
rect(yart+2*b, xart+23*b,b,b)
fill(af)
rect(yart+3*b, xart+23*b,b,b)
fill(af)
rect(yart+4*b, xart+23*b,b,b)
fill(af)
rect(yart+5*b, xart+23*b,b,b)
fill(af)
rect(yart+6*b, xart+23*b,b,b)
fill(af)
rect(yart+7*b, xart+23*b,b,b)
fill(af)
rect(yart+8*b, xart+23*b,b,b)
fill(af)
rect(yart+9*b, xart+23*b,b,b)
fill(af)
rect(yart+10*b, xart+23*b,b,b)
fill(aa)
rect(yart+11*b, xart+23*b,b,b)

//twaalfde laag 

fill(ac)
rect(yart-3*b, xart+24*b,b,b)
fill(aa)
rect(yart-2*b, xart+24*b,b,b)
fill(aa)
rect(yart-1*b, xart+24*b,b,b)
fill(aa)
rect(yart-0*b, xart+24*b,b,b)
fill(aa)
rect(yart+1*b, xart+24*b,b,b)
fill(aa)
rect(yart+2*b, xart+24*b,b,b)
fill(aa)
rect(yart+3*b, xart+24*b,b,b)
fill(aa)
rect(yart+4*b, xart+24*b,b,b)
fill(af)
rect(yart+5*b, xart+24*b,b,b)
fill(af)
rect(yart+6*b, xart+24*b,b,b)
fill(af)
rect(yart+7*b, xart+24*b,b,b)
fill(af)
rect(yart+8*b, xart+24*b,b,b)
fill(aa)
rect(yart+9*b, xart+24*b,b,b)
fill(aa)
rect(yart+10*b, xart+24*b,b,b)
fill(aa)
rect(yart+11*b, xart+24*b,b,b)

// elfde laag

fill(af)
rect(yart-2*b, xart+25*b,b,b)
fill(ag)
rect(yart-1*b, xart+25*b,b,b)
fill(ag)
rect(yart+0*b, xart+25*b,b,b)
fill(aa)
rect(yart+1*b, xart+25*b,b,b)
fill(aa)
rect(yart+2*b, xart+25*b,b,b)
fill(ai)
rect(yart+3*b, xart+25*b,b,b)
fill(aa)
rect(yart+4*b, xart+25*b,b,b)
fill(aa)
rect(yart+5*b, xart+25*b,b,b)
fill(aa)
rect(yart+6*b, xart+25*b,b,b)
fill(aa)
rect(yart+7*b, xart+25*b,b,b)
fill(aa)
rect(yart+8*b, xart+25*b,b,b)
fill(aa)
rect(yart+9*b, xart+25*b,b,b)
fill(ah)
rect(yart+10*b, xart+25*b,b,b)

//dertiende laag

fill(af)
rect(yart-2*b, xart+26*b,b,b)
fill(af)
rect(yart-1*b, xart+26*b,b,b)
fill(ag)
rect(yart-0*b, xart+26*b,b,b)
fill(ag)
rect(yart+1*b, xart+26*b,b,b)
fill(aa)
rect(yart+2*b, xart+26*b,b,b)
fill(aa)
rect(yart+3*b, xart+26*b,b,b)
fill(aa)
rect(yart+4*b, xart+26*b,b,b)
fill(aa)
rect(yart+5*b, xart+26*b,b,b)
fill(aa)
rect(yart+6*b, xart+26*b,b,b)
fill(aa)
rect(yart+7*b, xart+26*b,b,b)
fill(aa)
rect(yart+8*b, xart+26*b,b,b)
fill(aa)
rect(yart+9*b, xart+26*b,b,b)
fill(ac)
rect(yart+10*b, xart+26*b,b,b)

//veertiende

fill(ag)
rect(yart+0*b, xart+27*b,b,b)
fill(ag)
rect(yart+1*b, xart+27*b,b,b)
fill(ag)
rect(yart+2*b, xart+27*b,b,b)
fill(aa)
rect(yart+3*b, xart+27*b,b,b)
fill(aa)
rect(yart+4*b, xart+27*b,b,b)
fill(aa)
rect(yart+5*b, xart+27*b,b,b)
fill(aa)
rect(yart+6*b, xart+27*b,b,b)
fill(ac)
rect(yart+7*b, xart+27*b,b,b)
fill(ad)
rect(yart+8*b, xart+27*b,b,b)

//vijftiende laag

fill(ag)
rect(yart+2*b, xart+28*b,b,b)
fill(ag)
rect(yart+3*b, xart+28*b,b,b)
fill(ac)
rect(yart+4*b, xart+28*b,b,b)
fill(ac)
rect(yart+5*b, xart+28*b,b,b)
fill(ad)
rect(yart+6*b, xart+28*b,b,b)
fill(ad)
rect(yart+7*b, xart+28*b,b,b)
        }
  mouse1.cursor();

	}
      
  if (credits === true) {
  noStroke()   
	mainMenu = false;
       fill('#00087E')
      rect(10,10,100,150)
      textSize(30);
      fill(255);
      text('credits', 15, 50)
      textSize(30);
      fill(255);
      text(':Teun', 15, 80)
      textSize(30);
      fill(255);
      text(':Mees', 15, 110)
      
      fill('#0208C8')
      rect(120,10,200,170)
      textSize(85);
      fill(255);
      text('Back', 123, 120)
      
      fill('#373DFA')
      rect(330,10,60,380)
      
      fill('#02055B')
      rect(10,190,310,200)
      textSize(90);
      fill(255);
      text('Thanks', 18, 315)
     
      fill('#02055B')
      rect(10,170,100,20)
//mouse
fill(0)
ellipse(mouseX, mouseY, 10, 10)
      }




  if (startGame === true){
    
      fill(255)
      textSize(30);
      text(score, 15, 30);
			//laat score zien 
  
      score += 1
        
    player1Wins = false;
    player2Wins = false;
    
    player1.display();
  	player1.move();
  
  	player2.display();
		player2.move();
  
  	dispenser.display();
    
  	ball1.display();
  	ball1.move();
    ball1.collisionDetectionPlayer1();
    ball1.collisionDetectionPlayer2();
    
    ball2.display();
  	ball2.move();
    ball2.collisionDetectionPlayer1();
    ball2.collisionDetectionPlayer2();
    
    ball3.display();
  	ball3.move();
    ball3.collisionDetectionPlayer1();
    ball3.collisionDetectionPlayer2();
    
    ball4.display();
  	ball4.move();
    ball4.collisionDetectionPlayer1();
    ball4.collisionDetectionPlayer2();
    
    ball5.display();
  	ball5.move();
    ball5.collisionDetectionPlayer1();
    ball5.collisionDetectionPlayer2();
  	
    ball6.display();
  	ball6.move();
    ball6.collisionDetectionPlayer1();
    ball6.collisionDetectionPlayer2();
    
  	mainMenu = false;
    
  } 
  
  if (player1Wins === true){
    player1Win.display();
    
        
        fill(255)
      textSize(30);
      text(score, 15, 30);
			//laat score zien
    mouse1.cursor();
    
    startGame = false;
  }
  
  if (player2Wins === true){
    player2Win.display();
    
    fill(255)
      textSize(30);
      text(score, 15, 30);
			//laat score zien
        
        mouse1.cursor();
    
    startGame = false;
  }
}

class player{
  constructor(){
  	this.xPos = 350;
  	this.yPos = 350;
  	this.radius = 10;
    this.speed = 5;
	}
  
  display(){
    fill('#ff0000');
    ellipse(this.xPos, this.yPos, 2*this.radius, 2*this.radius);
  }

  move(){
 		if (keyIsDown (37) && this.xPos > 0 + this.radius) {
    			this.xPos -= this.speed;
  	}

		if (keyIsDown(39) && this.xPos < width - this.radius) {
    			this.xPos += this.speed;
    }

  	if (keyIsDown(38) && this.yPos > 0 + this.radius) {
    			this.yPos -= this.speed;
		}

    if (keyIsDown(40) && this.yPos < height - this.radius) {
    			this.yPos += this.speed;
		}
    
    if (this.xPos > width - this.radius ){
      this.xSpeed = -this.xSpeed;
    }
    if (this.yPos > height - this.radius ){
        this.ySpeed = -this.ySpeed;
    }
    if (this.xPos < 0 + this.radius){
    		this.xSpeed = -this.xSpeed
    }
    if (this.yPos < 0 + this.radius){
    		this.ySpeed = -this.ySpeed
    }
 	} 
}

class player0 {
  constructor(){
    this.xPos = 50;
    this.yPos = 50
    this.radius = 10;
    this.speed = 5;
  }
  
  display(){
    fill('#0000ff');
    ellipse(this.xPos, this.yPos, 2*this.radius, 2*this.radius);
  }
  
  move(){
 		if (keyIsDown (65) && this.xPos > 0 + this.radius) {
    			this.xPos -= this.speed;
  	}

		if (keyIsDown(68) && this.xPos < width - this.radius) {
    			this.xPos += this.speed;
    }

  	if (keyIsDown(87) && this.yPos > 0 + this.radius) {
    			this.yPos -= this.speed;
		}

    if (keyIsDown(83) && this.yPos < height - this.radius) {
    			this.yPos += this.speed;
		}
    
    if (this.xPos > width - this.radius || this.xPos < this.radius){
      this.xSpeed = -this.xSpeed;
    }
    if (this.yPos > height - this.radius || this.yPos < this.radius){
        this.ySpeed = -this.ySpeed;
    }
 	} 
}

class mouse {
  cursor() {
    fill(0);
    ellipse(mouseX, mouseY, 10, 10);
  }  
}

class art {
  display() {
		fill('#ff0000') 
    noStroke()
		rect(xDispenser, yDispenser, blok, blok)
		fill('#010000') 
    noStroke()
		rect(xDispenser + blok, yDispenser+blok, blok, blok)
		fill('#ff0000')
    noStroke()
		rect(xDispenser, yDispenser+blok, blok, blok)
		fill('#010000')
    noStroke()
		rect(xDispenser+blok, yDispenser, blok, blok)
		fill('#ff0000')
    noStroke()
		rect(xDispenser, yDispenser+2*blok, blok, blok)
		fill('#ff0000')
    noStroke()
		rect(xDispenser+blok, yDispenser+2*blok, blok, blok)
		fill('#0aa00a')
    noStroke()
		rect(xDispenser, yDispenser+3*blok, blok, blok)
		fill('#0aa00a')
    noStroke()
		rect(xDispenser+blok, yDispenser+3*blok, blok, blok)
		fill('#ff0000')
    noStroke()
		rect(xDispenser, yDispenser+4*blok, blok, blok)
		fill('#0aa00a')
    noStroke()
		rect(xDispenser+blok, yDispenser+4*blok, blok, blok)
		fill('#0aa00a')
    noStroke()
		rect(xDispenser+2*blok, yDispenser, blok, blok)
		fill('#010000')
    noStroke()
		rect(xDispenser+3*blok, yDispenser, blok, blok)
		fill('#010000')
    noStroke()
		rect(xDispenser+2*blok, yDispenser+blok, blok, blok)
		fill('#010000')
    noStroke()
		rect(xDispenser+2*blok, yDispenser+2*blok, blok, blok)
		fill('#010000')
    noStroke()
		rect(xDispenser+2*blok, yDispenser+3*blok, blok, blok)
		fill('#010000')
    noStroke()
		rect(xDispenser+3*blok, yDispenser+blok, blok, blok)
		fill('#0aa00a')
    noStroke()
		rect(xDispenser+2*blok, yDispenser+4*blok, blok, blok)
		fill('#0aa00a')
    noStroke()
		rect(xDispenser+3*blok, yDispenser+4*blok, blok, blok)
		fill('#0aa00a')
    noStroke()
		rect(xDispenser+4*blok, yDispenser+3*blok, blok, blok)
		fill('#0aa00a')
    noStroke()
		rect(xDispenser+3*blok, yDispenser+3*blok, blok, blok)
		fill('#ff0000')
    noStroke()
		rect(xDispenser+4*blok, yDispenser+4*blok, blok, blok)
		fill('#ff0000')
    noStroke()
		rect(xDispenser+4*blok, yDispenser+2*blok, blok, blok)
		fill('#ff0000')
    noStroke()
		rect(xDispenser+4*blok, yDispenser+blok, blok, blok)
		fill('#ff0000')
    noStroke()
		rect(xDispenser+4*blok, yDispenser, blok, blok)
		fill('#ff0000')
    noStroke()
		rect(xDispenser+3*blok, yDispenser+2*blok, blok, blok)       
	}

}

class ball{
	constructor(){
    this.xPos = width/2;
    this.yPos = height/2;
    this.radius = 10
    this.xSpeed = random(-3, 3);
    this.ySpeed = random(-3, 3);
  }

  display(){
    fill(random(0, 255), random(0, 255), random(0, 255))
  	ellipse(this.xPos, this.yPos, 2*this.radius, 2*this.radius);
  }

	move(){
    this.xPos += this.xSpeed;
    this.yPos += this.ySpeed;
    
    if (this.xPos < 0 - 2*this.radius ||
       this.xPos > width + 2* this.radius){
    	this.xPos = width/2;
      this.yPos = height/2;
      this.xSpeed = random(-3, 3);
    	this.ySpeed = random(-3, 3);
    }
    if (this.yPos < 0 - 2*this.radius ||
       this.yPos > height + 2*this.radius){
    	this.xPos = width/2;
      this.yPos = height/2;
      this.xSpeed = random(-3, 3);
    	this.ySpeed = random(-3, 3);
    }
  }
  
  collisionDetectionPlayer1(player){
  	var dx = this.xPos - player1.xPos;
	var dy = this.yPos - player1.yPos;
	if (sqrt(dx*dx + dy*dy) <= radius + radius){
      player1Wins = true;
      console.log('Player1 wins!'); 
    }
  }
  
  collisionDetectionPlayer2(player0){
  	var dx = this.xPos - player2.xPos;
		var dy = this.yPos - player2.yPos;
		if (sqrt(dx*dx + dy*dy) <= radius + radius){
      player2Wins = true;
      console.log('Player2 wins'); 
    }
  }
}

class playerWins{
	display(){  
    textSize(50);
    fill('#0000ff');
  	text('Player 1 wins!', 50, 150);
    
    noStroke();
    fill('#0000ff');
    rect(width/2 - 50, height/2, 100, 55);
    textSize(20);
    fill(0);
    text('Restart', 169, 235);
    
    noStroke();
    fill('#0000ff');
    rect(width/2 - 50, height/2 + 75, 100, 55);
    textSize(20);
    fill(0);
    text('Quit', 180,310);
  }
}

class player0Wins{
	display(){
    
  	textSize(50);
    fill('#ff0000');
  	text('Player 2 wins!', 50, 150);
    
    noStroke();
    fill('#ff0000');
    rect(width/2 - 50, height/2, 100, 55);
    textSize(20);
    fill(0);
    text('Restart', 169, 235);
    
    noStroke();
    fill('#ff0000');
    rect(width/2 - 50, height/2 + 75, 100, 55);
    textSize(20);
    fill(0);
    text('Quit', 180, 310);
  }
}

function mouseClicked() {
  if (mainMenu == true&&
    	mouseX > 170 &&
     	mouseX < 170 + 220 &&
     	mouseY > 10 &&
     	mouseY < 10 + 100){
	player1Wins = false;
	player2Wins = false;
	startGame = true;
      credits = false;
  }
  
  if (player1Wins == true &&
      mouseX > width/2 - 50 &&
      mouseX < width/2 - 50 + 100 &&
      mouseY > height/2 &&
      mouseY < height/2 + 55){
	player1Wins = false;
	player2Wins = false;
	startGame = true;	
	credits = false;

  }
  
  if (player2Wins == true &&
      mouseX > width/2 - 50 &&
      mouseX < width/2 - 50 + 100 &&
      mouseY > height/2 &&
      mouseY < height/2 + 55){
	player1Wins = false;
	player2Wins = false;
      startGame = true;
      credits = false;
  }
  
  if (player1Wins == true &&
      mouseX > width/2 - 50 &&
      mouseX < width/2 - 50 + 100 &&
      mouseY > height/2 + 75 &&
      mouseY < height/2 + 75 + 55){
    player1Wins = false;
    player2Wins = false;
    mainMenu = true;
      credits = false;
  }
  
  if (player2Wins == true &&
      mouseX > width/2 - 50 &&
      mouseX < width/2 - 50 + 100 &&
      mouseY > height/2 + 75 &&
      mouseY < height/2 + 75 + 55){
    player1Wins = false;
    player2Wins = false;
    mainMenu = true;
      credits = false;
  }

  if (mainMenu == true&&
    	mouseX > 10 &&
     	mouseX < 10 + 150 &&
     	mouseY > 10 &&
     	mouseY < 10 + 60){
	player1Wins = false;
	player2Wins = false;
	startGame = false;
      credits = true;
  }
      
      if (credits == true&&
    	mouseX > 120 &&
     	mouseX < 120 + 200 &&
     	mouseY > 10 &&
     	mouseY < 10 + 170){
	player1Wins = false;
	player2Wins = false;
	startGame = false;
      credits = false;
      mainMenu = true;
  }
}
