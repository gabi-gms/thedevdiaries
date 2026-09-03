# Exercício realizado no dia: 03/09/2026

> `Codewars` `Java` `String`

## Problema

Check to see if a string has the same amount of 'x's and 'o's. The method must return a boolean and be case insensitive. The string can contain any char.  


Examples input/output:  

```
XO("ooxx") => true  
XO("xooxx") => false
XO("ooxXm") => true
XO("zpzpzpp") => true // when no 'x' and 'o' is present should return true
XO("zzoo") => false
```

## Minha Solução

```
public class XO {
  
  public static boolean getXO (String str) {
    
    int countX = 0;
    int countO = 0;
    
    boolean sameAmount = false;
    
    for (int i = 0; i < str.length(); i++) {
      if (str.charAt(i) == 'x' || str.charAt(i) == 'X') {
        countX++;
      }else if (str.charAt(i) == 'o' || str.charAt(i) == 'O') {
        countO++;
      }
    }
    
    sameAmount = countX == countO ? true : false;
    
    return sameAmount;
    
  }
}
```

## Solução Otimizada

> Aqui vai uma versão não autoral mais otimizada de exemplo, conferida após a prática para comparação

```
public class XO {
  
  public static boolean getXO (String str) {
    
        long countX = str.toLowerCase().chars().filter(ch -> ch =='x').count();
        long countO = str.toLowerCase().chars().filter(ch -> ch =='o').count();

        return (countO==countX);
    
  }
}
```