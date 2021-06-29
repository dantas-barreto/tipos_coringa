# Tipos Coringa

### Generics são invariantes
`List<Object>` não é o supertipo de qualquer tipo de lista:  
  
`List<Object> myObjs = new ArrayList<Object>();`  
`List<Integer> myNumbers = new ArrayList<Integer>();`  
`myObjs = myNumbers;` // erro de compilação  
  
O supertipo de qualquer lista é `List<?>`. Este é um tipo coringa:  
  
`List<?> myObjs = new ArrayLIst<Object>();`  
`List<Integer> mynNumbers = new ArrayList<Integer>();`  
`myObjs = myNumbers;`
