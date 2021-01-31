# b-i-t-p-java-.package btvn;

import java.util.Iterator;
import java.util.Scanner;

public class bt_chuong2 {

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
//	        System.out.println("Trung bình cộng = " +tbc);
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
	             
	        // duyệt từ đầu đến cuối chuỗi
	        for (int i = 0; i < chuoi.length(); i++) {
	            // Nếu ký tự tại vị trí thứ i bằng 'a' thì tăng count lên 1
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
		             
		        // khai báo ma trận A có m dòng, n cột
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
