package sample;

public class Ball {
    private String color;
    private double radius;

    public Ball(String c, double r){
        color = c;
        radius = r;
    }
    public Ball(String c){
        color = c;
        radius = 0;
    }
    public Ball(){
        color = "blue";
        radius = 0;
    }
    public void setColor(String color){
        this.color = color;
    }
    public void setRad(double rad){
        this.radius = rad;
    }
    public String getColor() {
        return color;
    }
    public double getRad() {
        return radius;
    }
    public String toString() {
        return ("color of your ball: " + getColor() + "; Radius of your ball: " + getRad());
    }
}

package sample;

public class TestBall {
    public static void main (String [] args) {
        Ball b1 = new Ball("green", 1.1);
        Ball b2 = new Ball();
        Ball b3 = new Ball("black");
        System.out.println(b1.toString());
        System.out.println(b2.toString());
        System.out.println(b3.toString());
    }

}