###  [Task 7kyu](https://www.codewars.com/kata/542c0f198e077084c0000c2e/train/java)

Count the number of divisors of a positive integer n.
### My solution
```Java
public class FindDivisor {

    public long numberOfDivisors(int n) {
        int k=0;
        for(int i=1;i<=n;i++){
            if (n%i == 0){
                k++;}
        }
        return k;
    }

}
```

### Fav solution

```Java
import java.util.stream.IntStream;
public class FindDivisor {
    public long numberOfDivisors(int n) {
        return IntStream.range(1, n+1).filter(i -> n%i==0).count();
    }
}
```
I like this solution because I like it
