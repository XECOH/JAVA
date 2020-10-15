# 1928. Base64 Decoder



### Java

```java
import java.util.Scanner;
import java.util.Base64;
import java.util.Base64.Decoder;

class Solution {
  public static void main(String args[]) {
    Scanner sc = new Scanner(System.in);
    Decoder decoder = Base64.getDecoder();
    int T = sc.nextInt();
    for (int tc=1; tc<=T; tc++) {
      String str = sc.next();
			byte[] decoded = decoder.decode(str);
      System.out.printf("#%d %s\n", tc, new String(decoded));
    }
  } 
}
```

