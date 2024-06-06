# Frequency
Frequency of limited array range elements
#include<iostream>
using namespace std;

int main(){
	int n;
	cout<<"Enter the size: ";
	cin>>n;
	int arr[n];
	for(int i=0;i<n;i++){
		cin>>arr[i];
	}
	int m=arr[0];
	for(int i=0;i<n;i++){
		if(arr[i]>m){
			m=arr[i];
		}
	}
	int freq[m]={0};
	for(int i=0;i<n;i++){
		freq[arr[i]-1]++;
	}
	for(int i=0;i<m;i++){
		cout<<freq[i]<<" ";
	}
}
