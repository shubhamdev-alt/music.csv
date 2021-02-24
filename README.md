# music.csv
it is an program for read csv file and output in increasing order
import java.io.BufferedReader;  
import java.io.FileReader;  
import java.io.IOException;  
public class ReadCSVExample2  
{  
public static void main(String[] args)   
{  
String line = "";  
String splitBy = ",";  
try   
{  
//parsing a CSV file into BufferedReader class constructor  
BufferedReader br = new BufferedReader(new FileReader("music.csv"));  
while ((line = br.readLine()) != null)   //returns a Boolean value  
{  
String[] music = line.split(splitBy);    // use comma as separator  
System.out.println("Employee [Song Name=" + music[0] + ", artist Name=" + music[1] +]");  
}  
}   
catch (IOException e)   
{  
e.printStackTrace();  
}  
}  
}  


//output
Memories, Maroon 5, 3:09
Bad guy, Billie Eilish, 3:14
Blinding Lights, The Weeknd, 3:20

