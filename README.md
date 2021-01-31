package btvn;

import java.util.Iterator;
import java.util.Scanner;

public class bt_chuong2 {

    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        System.out.println("nhap so a: ");
        int a = sc.nextInt();
        System.out.println("nhap so b: ");
        int b = sc.nextInt();
        int tong = a+b;
        int hieu = a-b;
        int tich = a*b;
        int thuong = a%b; 
        System.out.println("tong la: " +tong);
        System.out.println("hieu la: " +hieu);
        System.out.println("tich la: " +tich);
        System.out.println("thuong la:" +thuong);
        int max = a>b ? a:b;
        System.out.println("so lon hon la: " + max);
    sc.close();
    }
//bai 2
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        System.out.println("nhap so n: ");
        int n = sc.nextInt();
        if( n%2 ==0){
            System.out.println("so chan");
        }else{
            System.out.println("so le");
        }
        sc.close();
    }
//bai3
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        System.out.println("nhap ten cua ban: ");
        String ten = sc.next(); 
        System.out.println("nhap nam sinh cua ban: ");
        int ns = sc.nextInt();
        int tuoi = 2020 - ns;
        if(tuoi < 16){
            System.out.println("ban " +ten + " o do tuoi vi thanh nien");
        }else if(tuoi >=16){
            System.out.println("ban " +ten +" o do tuoi truong thanh");
        }else if(tuoi >= 18){
            System.out.println("ban " +ten +" o do tuoi gia");
        }
        sc.close();
    }
//bai4
 public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        System.out.println("nhap vao mot so: ");
        int month = sc.nextInt();
        if(month<=0||month>12){
            System.out.println("thang khong hop le");
        }
            switch(month){
                case 1:System.out.println("thang mot");
                break;
                case 2:System.out.println("thang hai");
                break;
                case 3:System.out.println("thang ba");
                break;
                case 4:System.out.println("thang tu");
                break;
                case 5:System.out.println("thang nam");
                break;
                case 6:System.out.println("thang sau");
                break;
                case 7:System.out.println("thang bay");
                break;
                case 8:System.out.println("thang tam");
                break;
                case 9:System.out.println("thang chin");
                break;
                case 10:System.out.println("thang muoi");
                break;
                case 11:System.out.println("thang muoi mot");
                break;
                case 12:System.out.println("thang muoi hai");
                break;
            }
        sc.close();
    }
//bai5
public static void main(String[] args) throws Exception {
        int s = 0;
        int n;
        Scanner sc = new Scanner(System.in);
        do {
            System.out.println("nhap n: ");
             n = sc.nextInt();
            s += n;
    }while(s < 100);
    sc.close();
    System.out.println("Tong la: " +s);
    }
//bai6
    Scanner sc = new Scanner(System.in);
        System.out.println("Nhập vào một số nguyên dương: ");
        int a = sc.nextInt();
        int b = 1;
        int i = 1;
        do{
            b*=i;
            i++;
        }while(i<=a);
        System.out.println("Giai thừa là: "+b);
        sc.close();
    }
	public static void main(String[] args) {
		//bai 7
		for (int i=0;i<=19;i++) {
			System.out.println("20 so nguyen duong dau tien la: "+i);
			
		}
//		//bai 8
		int n, tuso=0;
		int tbc;
		  Scanner sc = new Scanner(System.in);
	         
	        
	         
	        System.out.println("Nhập vào số các số nguyên có trong dãy: ");
	        n = sc.nextInt();
	         

	        for (int count = 1; count <=n; count++) {
	            System.out.println("Nhập số thứ " + count + ": ");
	            n = sc.nextInt();
	           tuso += n;
	        }
	         
	        tbc = tuso/ n;
	        System.out.println("Trung bình cộng = " +tbc);
//	        //bai9
	        String chuoi;
	        char kyTu;
	        Scanner scanner = new Scanner(System.in);
	             
	        System.out.println("Nhập vào chuỗi bất kỳ: ");
	        chuoi = sc.nextLine();
	             
	        System.out.println("Các ký tự có trong chuỗi là: ");
	        for (int i = 0; i < chuoi.length(); i++) {
	            
	            kyTu = chuoi.charAt(i);
	                 
	            System.out.println(kyTu);
	        }
//	        //bai10
	        String chuoi;
	        char kyTu = 'a';
	        int count = 0;
	        Scanner scanner = new Scanner(System.in);
	             
	        System.out.println("Nhập vào chuỗi bất kỳ: ");
	        chuoi = scanner.nextLine();
	             
	       
	        for (int i = 0; i < chuoi.length(); i++) {
	           
	            if (chuoi.charAt(i) == kyTu) {
	                count++;
	            }
	        }
	             
	        System.out.println("Số lần xuất hiện của ký tự " + kyTu +
	            " trong chuỗi " + chuoi + " = " + count);
		//bai11
		
		 
		 
	
		
		    Scanner scanner= new Scanner(System.in);
		     
		
		
		        System.out.print("Nhập số phần tử của mảng: ");
		        int n =scanner.nextInt();
		      
		        int [] arr = new int [n];
		        System.out.print("Nhập các phần tử của mảng: \n");
		        for (int i = 0; i < n; i++) {
		            System.out.printf("a[%d] = ", i);
		            arr[i] = scanner.nextInt();
		        }
		   
		        sortASC(arr);
		        System.out.println("Dãy số được sắp xếp tăng dần: ");
		        show(arr);
		    }
		     
		   
		    public static void sortASC(int [] arr) {
		        int temp = arr[0];
		        for (int i = 0 ; i < arr.length - 1; i++) {
		            for (int j = i + 1; j < arr.length; j++) {
		                if (arr[i] > arr[j]) {
		                    temp = arr[j];
		                    arr[j] = arr[i];
		                    arr[i] = temp;
		                }
		            }
		        }
		    }
		     
		   
		    public static void show(int [] arr) {
		        for (int i = 0; i < arr.length; i++) {
		            System.out.print(arr[i] + " ");
		        }
//		        //bai12
		        int m, n;
		         
		        Scanner scanner = new Scanner(System.in);
		             
		        System.out.println("Nhập vào số dòng của ma trận: ");
		        m = scanner.nextInt();
		        System.out.println("Nhập vào số cột của ma trận: ");
		        n = scanner.nextInt();
		             
		       
		        int A[][] = new int[m][n];
		             
		        System.out.println("Nhập các phần tử cho ma trận: ");
		        for (int i = 0; i < m; i++) {
		            for (int j = 0; j < n; j++) {
		                System.out.print("A[" + i + "]["+ j + "] = ");
		                A[i][j] = scanner.nextInt();
		            }
		        }
		             
		     
		        int max = A[0][0];
		             
		        for (int i = 0; i < m; i++) {
		            for (int j = 0; j < n; j++) {
		                if (max < A[i][j]) {
		                    max = A[i][j];
		                }
		            }
		        }
		             
		        System.out.println("Phần tử lớn nhất trong ma trận = " + max);
		    
		    }
	
		   
	
	    }
	        
	 
