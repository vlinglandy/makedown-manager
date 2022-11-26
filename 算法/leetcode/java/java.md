```
public class Test {

    static int max;
    static int k;
    static int x;
    static boolean flag=true;
    static int sum=0;
    static int[] arr;
    static int[] record;
    public static void dfs(int n,int sum) {
        if(n==max){
            if(sum==x){
                flag=false;
                for (int i = 0; i < n; i++) {
                    System.out.print(arr[i]+" ");
                }
                System.exit(1);
            }
            return ;
        }
        for (int i = 1; i <= k; i++) {
            if(record[i]==0){
                arr[n]=i;
                record[i]=1;
                sum+=i;
                dfs(n+1,sum);
                sum-=i;
                record[i]=0;
                arr[n]=0;
            }
        }
    }


    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

         max=sc.nextInt();
         k=sc.nextInt();
         x=sc.nextInt();
        if(max*k<x) {
            System.out.println(-1);
            return;
        }
        arr=new int[k];
        record=new int[k+1];
        dfs(0,0);
        if(flag) {
            System.out.println(-1);
        }
    }
}
```
