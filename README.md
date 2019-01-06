/* First lets set a background */
.bg{
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: url('https://images.unsplash.com/photo-1431352832634-845fad190fbd?ixlib=rb-0.3.5&q=80&fm=jpg&crop=entropy&s=ec80c41e488dc2b99ed543df2f3f0919');
  background-position: center center;
  background-origin: content-box;
  background-size: cover;
  background-attachment: fixed;
  z-index: -2;
}

/* Now the same background, but with brightness filters*/
.lightning{
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: url('https://images.unsplash.com/photo-1431352832634-845fad190fbd?ixlib=rb-0.3.5&q=80&fm=jpg&crop=entropy&s=ec80c41e488dc2b99ed543df2f3f0919');
  background-position: center center;
  background-origin: content-box;
  background-size: cover;
  background-attachment: fixed;
  -webkit-filter: brightness(3);
  filter: brightness(3);
  -o-filter: brightness(3);
  -moz-filter: brightness(3);
  z-index: -1;
}

/*Now just a opacity animation*/
.flashit{
-webkit-animation: flash ease-out 7s infinite;
animation: flash ease-out 7s infinite;
-webkit-animation-delay: 2s;
        animation-delay: 2s;
}

@-webkit-keyframes flash {
	from { opacity: 0; } 
  92% { opacity: 0; }
	93% { opacity: 0.6; }
  94% { opacity: 0.2; }
  96% { opacity: 0.9; } 
	to { opacity: 0; }
}

@keyframes flash {
	from { opacity: 0; } 
    92% { opacity: 0; }
	93% { opacity: 0.6; }
    94% { opacity: 0.2; }
    96% { opacity: 1; } 
	to { opacity: 0; }
}
/*End! is that simple! */

/*Now just some stupid logo to get some look and feel */
#logo{
  z-index:1000;
  width: 100%;
  font-size: 6rem;
  color: white;
  position: fixed;
  top: 50%;
  left: 50%;
  margin-left: -18rem;
  margin-top: -2rem;
  font-weight: 900;
}
#logo span{ font-weight: 100;}

html , body{
  font-family: "Titillium Web", "lato" , sans-serif;
}
@import url(https://fonts.googleapis.com/css?family=Titillium+Web:200,900|Lato:100,300,900);

@media screen and (max-width: 630px){
  #logo{
    font-size: 3rem;
    margin-left: -9rem;
    margin-top: -1rem;
  }
}
