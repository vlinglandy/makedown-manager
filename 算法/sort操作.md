## sort比较多维vector

```cpp
sort(intervals.begin(),intervals.end(),[](vector<int> &a,vector<int> &b){
    return a[1]<b[1];
});
```

```java
  Arrays.sort(ins, (a, b)->{
            return a[1] != b[1] ? a[1] - b[1] : b[0] - a[0];
        });
```
