#include<iostream.h>
#include<conio.h>
#include<stdio.h>
#include<string.h>
#include<stdlib.h>
#include<fstream.h>
void adddata(void);
void show(void);
void seardata(char [] , char [], char []);

struct flight
{
	int fno,deti,arti,pr,d1,d2;
	char air[100],dest[100],src[100],dedt[100],ardt[100];
}f[100];

void addata()
{
	clrscr();
	int i=0;
	char cha;
	char ch='y';
	cout<<"Enter Details of Flight\n\n";
	while (ch=='y')
	{
		clrscr();
		cout<<"\nEnter Flight Number::";
		cin>>f[i].fno;
		cout<<"Enter Airline Name::";
		gets(f[i].air);
		cout<<"Enter Airline Destination::";
		gets(f[i].dest);
		cout<<"Enter Airline Source::";
		gets(f[i].src);
		cout<<"Enter Airline Departure Date::";
		gets(f[i].dedt);
		cout<<"Enter Airline Departure Time::";
		cin>>f[i].deti;
		cout<<"Enter Airline Arrival Date::";
		gets(f[i].ardt);
		cout<<"Enter Airline Arrival Time::";
		cin>>f[i].arti;
		cout<<"Enter Airline Price::";
		cin>>f[i].pr;
		cout<<"\n\nEnter More Data(y/n)::";
		ch=getche();
		if(ch=='n')
		{
			show();
		}
		i++;
	}
}

void seardata()
{
	clrscr();
	char dest[100];
	char ddate[100],adate[100];
	cout<<"\n\n\t\tEnter Your Data::\n\n";
	cout<<"\t\t1) Destination::";
	gets(dest);
	cout<<"\t\t2) Departure Date::";
	gets(ddate);
	cout<<"\t\t3) Arrival Date::";
	gets(adate);
	clrscr();
	cout<<"\n\t\tFlight List Is as Follows::\n";
	int i=0;
		if(strcmp(f[i].dedt,ddate)==0)
		{
			cout<<f[i].fno<<"\n";
			puts(f[i].air);
			cout<<"\n";
			puts(dest);
			cout<<f[i].pr;
			cout<<"\n";
			puts(f[i].src);
			cout<<"\n\n";
		}
	cout<<"\n\t\tEnter the Fliter:--";
	cout<<"\n\t\t1)Price";
	cout<<"\n\t\t2)Destination";
	cout<<"\n\t\t3)Source";
	cout<<"\nEnter choice::";
	char ch;
	cin>>ch;
	cout<<"\n\t\tFlight List Is as Follows::\n";
	i=0;
		if(strcmp(f[i].dedt,ddate)==0)
		{
			cout<<f[i].fno<<"\n";
			puts(f[i].air);
			cout<<"\n";
			puts(dest);
			cout<<"\n"<<f[i].pr;
			cout<<"\n";
			puts(f[i].src);
			cout<<"\n\n";
		}

}

void show()
{
	clrscr();
	int ch;
	cout<<"\t\t\tWELCOME TO FLIGHT BOOKING SYSTEM\n\n\n\n";
	cout<<"\t\t1)Add Data Of Flight\n\n";
	cout<<"\t\t2)Search Data For Flight\n\n";
	cout<<"\t\tEnter Your Choice::";
	cin>>ch;
	switch (ch)
	{
		case 1:
			addata();
			break;
		case 2:
			seardata();
			break;

	}
}

void main()
{
	clrscr();
	show();
	getch();
}
