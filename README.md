# Company
//This is something I am working on for my first course learning Java - it is only one part of the project 
public class Verwaltung {

	public final int SIZE = 12;
	private final Employees[] employee_list = new Employees[SIZE];
	
	  private void init() {
	  
	  employee_list[0] = new WorkfromHome(1, "Johann", 990, 120);
	  employee_list[1] = new WorkfromHome(2, "Maria", 880, 90);
	  employee_list[2] = new WorkfromHome(3, "Georg", 1200, 220);
	  employee_list[3] = new WorkfromHome(4, "Anna", 2200, 110);
	  employee_list[4] = new WorkfromHome(5, "Leo", 1300, 80);
	  employee_list[5] = new WorkfromHome(6, "Catharina", 2000, 300);
	  
	  employee_list[6] = new WorkNormally(7, "Jonathan", 8, 40, 100);
	  employee_list[7] = new WorkNormally(8, "Leonie", 7, 39, 70);
	  employee_list[8] = new WorkNormally(9, "Michalis", 15, 29, 250);
	  employee_list[9] = new WorkNormally(10, "Clara", 11, 30, 150);
	  employee_list[10] = new WorkNormally(11, "Markus", 7, 38, 25);
	  employee_list[11] = new WorkNormally(12, "Lisa", 13, 45, 230); 
	  } 
	
	public String employee_search() {	 
			 int search = 3;
			 
			 for(int i = 0; i < SIZE; i++) {
				 if(search == i)
					 System.out.println(employee_list[i+1]);					 
			 }			 
			 return super.toString();  
		  }
	
	public static void main(String[] args) {
		
		System.out.println(employee_list());    //getting an error message here:
                                             //cannot make a static reference to a non static method
                                              //what would be the easiest way to fix this?
		
	}
