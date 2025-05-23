# distance-calculator-
can calculate disance  btween 2 points 
#include<iostream>
#include<cmath>

using namespace std;
class point{
    int x, y;
    friend void distance(point, point);
    
    public:
    point(int a, int b){
        x = a;
        y = b; 
        
}
void displaypoint(){
    cout<<"the point is ("<<x<<","<<y<<")"<<endl;

}
};
void distance( point p1, point p2){
    double x_dist =  (p2.x - p1.x);
    double y_dist =  (p2.y - p1.y);
    double dist = sqrt(pow(x_dist,2) + pow(y_dist,2));
    cout<<"the distance is "<<dist<<endl;
}
int main(){
    point a(1,1);
    point b(2,4);
    
     distance(a,b);
    return 0;
};
