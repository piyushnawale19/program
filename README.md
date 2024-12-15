class Complex{
    float real;
    float img;
Complex(float real,float img){
    this.real=real;
    this.img=img;
}
Complex Add(Complex c1,Complex c2){
    Complex temp=new Complex(0,0);
    temp.real=c1.real+c2.real;
    temp.img=c1.img+c2.img;
    return temp;
}
Complex Sub(Complex c1,Complex c2){
    Complex temp=new Complex(0,0);
    temp.real=c1.real-c2.real;
    temp.img=c1.img-c2.img;
    return temp;
}
Complex Mul(Complex c1,Complex c2){
    Complex temp=new Complex(0,0);
    temp.real=c1.real*c2.real;
    temp.img=c1.img*c2.img;
    return temp;
}
Complex Div(Complex c1,Complex c2){
    Complex temp=new Complex(0,0);
    temp.real=c1.real/c2.real;
    temp.img=c1.img/c2.img;
    return temp;
}
void show(){
    System.out.println(real+"+"+img+"i");
}
}
public class Main{
    public static void main(String args[]){
        Complex c1=new Complex(10,30);
        Complex c2=new Complex(40,50);
        Complex c3=new Complex(0,0);
        c3=c3.Add(c1,c2);
        c3.show();
        c3=c3.Sub(c1,c2);
        c3.show();
        c3=c3.Mul(c1,c2);
        c3.show();
        c3=c3.Sub(c1,c2);
        c3.show();


    }
}
