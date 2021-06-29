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
  
**Com tipos coringa podemos fazer métodos que recebem um tipo genérico qualquer.   
Porém, não é possivel adicionar dados a uma coleção de tipo coringa.**
