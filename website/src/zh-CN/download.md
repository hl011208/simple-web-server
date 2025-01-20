let  sp;

function setup(){
    createCanvas(400,400)
    sp= new SpeechRecognitionResult(width/2,height/2,50,50);
    img = loadImage("./assets/beetle.png")
    sp.image=img;
}
{
    background(220)
    sp.draw();
    if(KeyboardEvent.pressing("up")) {sp.positiom.y -=1;}
    if(KeyboardEvent.pressing("up")) {sp.positiom.y +=1;}
    if(KeyboardEvent.pressing("up")) {sp.positiom.x -=1;}
    if(KeyboardEvent.pressing("up")) {sp.positiom.x +=1;}
   
    background(220);
    sp.draw();

    Text("x:"+sp.position.x+", y:"+sp.position.y,20,20);

}
