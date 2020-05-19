# Comparators

Comparators are an interface similar to comparable, only instead of using a comparable array, they accept an Object array, and a Comparator operator:

Comparable
`static void sort(Comparable[] a) { do the sort using less/swap functions using compareTo method of comparable }`

Comparator
`static void sort(Object[] a, Comparator comparator) { do the sort using less/swap functions using compare method of comparable }`

To define a comparator, you create private Comparator nested clas in your class which implements the compare method like so:


``` 
public class Student{
   public static final Comparator<Student> BY_NAME = new ByName();
   public static final Comparator<Student> BY_SECTION = new BySection();
   ...
   ...

   private static class ByName implements Comparator<Student> {
       public int compare(Student v, Student w){
           return v.name.compareTo(w.name);
   }   }

   private static class BySection implements comparator<Student>{
      public int compare ( Student v, Studentw) {
      return v.section - w.section }
   }
}

Now, you can pass Array.sory(a, Student.BY_NAME) to sort on different keys for the same data.

This has many applications for all sorts of data processing

