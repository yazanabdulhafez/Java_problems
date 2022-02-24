# Java_problems

## length of the last word in string

```java
public int lengthOfLastWord(String s) {
int count=0;
s=s.trim();
for(int i=s.length()-1;i>=0;i--){
  if(s.charAt(i)!=' ')
   count++;
  if(count!=0 && s.charAt(i)==' ')
  break;
}
return count; 
}
}
```

```java
 public int lengthOfLastWord(String s) {
        s = s.trim();
        String lastWord = s.substring(s.lastIndexOf(" ")+1, s.length());
        //System.out.println(lastWord);
        return lastWord.length();
    }

```
