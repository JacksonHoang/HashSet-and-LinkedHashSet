# HashSet-and-LinkedHashSet
HashSet allows no duplicates and order is not maintained. LinkedHashSet will maintain an insertion order.



import java.util.*;

class AceTester
{

	   public static void main(String args[]) {

		   //HashSet
		   HashSet haashSet = new HashSet();
		   haashSet.add("z"); //No duplicates allowed
		   haashSet.add("z"); //Order is not maintained
		   haashSet.add("z"); //z z z s c b a, will be ordered in a b s c z 
		   haashSet.add("s");
		   haashSet.add("c"); 
		   haashSet.add("b"); 
		   haashSet.add("a"); 
		   System.out.println("HashSet values are:" + haashSet);
		   
		   //LinkedHashSet
		   LinkedHashSet linkHS = new LinkedHashSet();
		   linkHS.add(5); //LinkedHashSet will maintain insertion order
		   linkHS.add(4); //Prints: 5 4 3 2 1
		   linkHS.add(3);
		   linkHS.add(2);
		   linkHS.add(1);
		   System.out.println("LinkedHashSet values are:" + linkHS);
		   }
       
}
