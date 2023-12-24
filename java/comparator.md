c

students.sort(Comparator.comparing(Student::getBirthDay,  
Comparator.nullsLast(Comparator.reverseOrder())));  
  
  
  
List.copyOf(sportList)