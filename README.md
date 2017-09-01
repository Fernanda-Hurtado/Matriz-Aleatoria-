# Matriz-Aleatoria-
//Maria Fernanda Hurtado Ruiz
int x=350;
int y=450;
int a=350;
int b=450;
int c=450;

void setup(){
  size(800,800);
  background(#92C9B7);
}
void draw(){

 if ((mouseX >=350 & mouseX <=450)& (mouseY >=350 & mouseY <=450)){
   x=x-1;
   y=y+1;
   a=a-1;
   b=b+1;
   c=c+1;
 }
 else {
   x=350;
   y=450;
   a=350;
   b=450;
   c=450;

 }
  triangulo(x,y,400,a,b,c);
 println(mouseX);
}


void triangulo(int x, int y, int z, int a, int b, int c){
  noStroke();
for(int i=350; i>=x; i=i-5){
  for(int q=450; q<=b; q=q+5){
    for(int r=450; r<=y; r=r+5){     
      fill(random(255));
      triangle(i, r, 400, a, q, c);
    }
  }
}
}
