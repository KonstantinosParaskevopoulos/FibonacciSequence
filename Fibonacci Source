#include <iostream>

using namespace std;
class FibonacciSeq{
public:
unsigned long long int n0, n1;
unsigned long long int next; //temporary result
unsigned long long int terms, i; //for the for loop
	FibonacciSeq(int fn0, int fn1){ //constructor for initialization of sequence
		n0=fn0;
		n1=fn1;
	}
void fibonacci(){ //sequence method
	cout<<"-----------Give number of terms: ";
	cin>>terms; //selection of terms to print
	for(i=1; i<=terms; i++){
		next=n0+n1;
		cout<<"Term "<<i<<": "<<next<<endl;
		n0=n1;
		n1=next;
	}
	system("PAUSE");
	system("cls");
}
void fibonwithstep(){
	unsigned long long int step;
	cout<<"--------Give number of terms: ";
	cin>>terms; //selection of terms to print
	cout<<"--------Give step: ";
	cin>>step; //selection of step
	for(i=1; i<=terms; i++){
		n1=n1+step;
		next=n0+n1;
		cout<<"--------Term "<<i<<": "<<next<<endl;
		n0=n1;
		n1=next;
	}
	system("PAUSE");
	system("cls");
}
};
class Menu{
	public:
	int choice;
	void menu(){
		do{
		cout<<"\t\tFibonacci Counter\n"<<endl;
		cout<<"-----------------------------------------------\n";
		cout<<"--------0.Exit\n";
		cout<<"--------1.Simple Fibonacci\n";
		cout<<"--------2.Fibonacci with Step\n";
		do{
		cout<<"--------Choose corresponding number: ";
		cin>>choice;
		system("cls");
		}while(choice>2&&choice<1);
		if(choice==1){
			FibonacciSeq fs(0,1);
			fs.fibonacci();
		}
		else if(choice==2){
			FibonacciSeq fss(0,0);
			fss.fibonwithstep();	
		}		
	}		while(choice!=0);
}
};

int main(){
	Menu m;
	m.menu();

	return 0;
}
