Question 2 :Best Time to Buy and Sell Stock

class buyasstock {
	int maxprofit(int a[]) {
		int maxprofit = 0;
		int minsofar = a[0];
		for ( int i=0; i<a.length; i++) {
			minsofar = Math.min(minsofar,a[i]);
			int profit = a[i] - minsofar;
			maxprofit = Math.max(maxprofit, profit);
			
		}
		return maxprofit;
		
	}
public static void main(String Args[]) {
	buyasstock buy = new buyasstock();
	int a[] = {7,1,5,3,6,4};
	System.out.println(buy.maxprofit(a));
	
}
}

Question 1 : Leader in the Array


import java.util.Arrays;

public class Arraysort {

	public static void main(String[] args) {
		
		int a[] = {5,6,20,6,2};
		int size = a.length;
		Arrays.sort(a);

		
		System.out.println( a[size-1]);
				
		
	}

}

Question 3:Sum of All Subset XOR Totals


public class XOR {
	 int xorSum(int a[], int n)
    {
         
        int bit = 0;
     
        
        for (int i = 0; i < n; ++i)
            bit |= a[i];
     
        int ans = bit * (int)Math.pow(2, n-1);
     
        return ans;
    }

	public static void main(String[] args) {
		XOR bitwise = new XOR();
		int a[] = {1, 3};
        int n = a.length;
         
        System.out.print(bitwise.xorSum(a, n));	

	}

}
