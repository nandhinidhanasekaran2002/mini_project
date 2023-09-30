# mini_project
package project;
import java.io.*;
import java.util.Scanner;
class details{
	public void show() {
		System.out.println("Welcome!!FANTASY LIGHTS Online Book Store");
		System.out.println("*****************************************");
		System.out.println("To create an Account for online shop!!");
	}
	public void AccountCreate() {
	System.out.println("Account create successfully!!");
	System.out.println("*****************************");
	
	}
}
public class Book {

	public static void main(String[] args)throws IOException {
		details D=new details();
		D.show();
		InputStreamReader is=new InputStreamReader(System.in);
		BufferedReader input=new BufferedReader(is);
		System.out.println("Enter your Name:");
		String name=input.readLine();
		
		System.out.println("Enter your password in Integer:");
		String A=input.readLine();
		int pass=Integer.parseInt(A);
		
		BufferedReader br=new BufferedReader(is);
		System.out.println("Enter your Gmail:");
		String mail=input.readLine();
		
		D.AccountCreate();
		System.out.println("User Name:"+name);
		System.out.println("User password:"+pass);
		System.out.println("Gmail:"+mail);
		
		while(true) {
			System.out.println("press 1 to check books available");
			System.out.println("press 2 to show details about book");
			System.out.println("press 3 to pay money for Book to get the Receipt");
			Scanner S=new Scanner(System.in);
			int opt=S.nextInt();
			switch(opt) 
			{
			case 1:
				System.out.println("The Autobiography Books:");
				System.out.println("************************");
				System.out.println("1.Wings of fire");
				System.out.println("2.India of my dreams");
				System.out.println("3.The discovery of India");
				System.out.println("4The god of small Things");
				System.out.println("5.The Indian Struggle");
				System.out.println("6.Courts and their Judgements");
				System.out.println("***************************");
				break;
			case 2:
				System.out.println("Books and Author");
				System.out.println("****************");
				System.out.println("1.Wings of fire------------------Author-Dr APJ Abdul Kalam");
				System.out.println("2.India of my dreams-------------Author-Mahatma Gandhi");
				System.out.println("3.The discovery of India---------Author-Jawaharlal Nehru");
				System.out.println("4.The god of small Things--------Author-Arundhati Nehru");
				System.out.println("5.The Indian Struggle------------Author-Subhas Chandra Bose");
				System.out.println("6.Courts and their Judgements----Author-Khushwant singh");
				System.out.println("***************************************************");
				break;
			case 3:
				System.out.println("Pay Money");
				System.out.println("*********");
				while(true) {
					System.out.println("press 1 to buy Wings of fire");
					System.out.println("press 2 to buy India of my dreams");
					System.out.println("press 3 to buy The discovery of India ");
					System.out.println("press 4 to buy The god of small Things");
					System.out.println("press 5 to buy The Indian Struggle");
					System.out.println("press 6 to buy Courts and their Judgements");
					Scanner scan=new Scanner(System.in);
					int option=scan.nextInt();
					switch(option) {
					case 1:
						int pay=1000;
						System.out.println("Wing of fire is Rs.1000");
						System.out.println("Enter the amount to pay:");
						int money=scan.nextInt();
						if(pay==money) {
							System.out.println("Succesfully paid");
							System.out.println("****************");
						}
						else {
							System.out.println("not paid");
						}
						break;
					case 2:
						int p=2000;
						System.out.println("India of my dreams is Rs.2000");
						System.out.println("Enter the amount to pay:");
						int M=scan.nextInt();
						if(p==M) {
							System.out.println("Succesfully paid");
							System.out.println("****************");
						}
						else {
							System.out.println("not paid");
						}
						break;
					case 3:
						int P=2500;
						System.out.println("The discovery of India is Rs.2500");
						System.out.println("Enter the amount to pay:");
						int bal=scan.nextInt();
						if(P==bal) {
							System.out.println("Succesfully paid");
							System.out.println("****************");
						}
						else {
							System.out.println("not paid");
						}
						break;
					case 4:
						int buy=3500;
						System.out.println("The god of small Things is Rs.3500");
						System.out.println("Enter the amount to pay:");
						int balance=scan.nextInt();
						if(buy==balance) {
							System.out.println("Succesfully paid");
							System.out.println("****************");
						}
						else {
							System.out.println("not paid");
						}
						break;
					case 5:
						int fare=3000;
						System.out.println("The Indian Struggle is Rs.3000");
						System.out.println("Enter the amount to pay:");
						int Bal=scan.nextInt();
						if(fare==Bal) {
							System.out.println("Succesfully paid");
							System.out.println("****************");
						}
						else {
							System.out.println("not paid");
						}
						break;
					case 6:
						int Fare=2500;
						System.out.println("Courts and their Judgements is Rs.4000");
						System.out.println("Enter the amount to pay:");
						int Money=scan.nextInt();
						if(Fare==Money) {
							System.out.println("Succesfully paid");
							System.out.println("****************");
						}
						else {
							System.out.println("not paid");
						}
						break;
					}
					break;
				}
			case 4:
				System.out.println("--------------------------------");
				System.out.println("Here, your receipt "+name);
				System.out.println("How  many books you bought:");
				int a=S.nextInt();
				System.out.println("how much cost you paid:");
				int b=S.nextInt();
				System.out.println("No of books\t\tTotalprice\t\t");
				System.out.println("-----------\t\t----------\t\t-");
				System.out.println(a+"\t\t\t"+b+"\t\t");
				System.out.println("--------------------------------");
				System.out.println("Thank you for Visting "+name);
				System.out.println("Come Again!!!");
				System.out.println("***************************");
				//break;
					
			}
			
		}
	}
}



	
	
	

