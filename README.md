<div align="center">

## User Input through Console


</div>

### Description

This is an example program shows how u can get input through the console window such as dos,etc. It may look silly example, but i am sure u will learn more from this, if u r a beginner. please vote me. thanks...
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[TheCodeGuru](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/thecodeguru.md)
**Level**          |Beginner
**User Rating**    |4.3 (13 globes from 3 users)
**Compatibility**  |Java \(JDK 1\.1\), Java \(JDK 1\.2\)
**Category**       |[Files/ File Controls/ Input/ Output](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/files-file-controls-input-output__2-58.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/thecodeguru-user-input-through-console__2-3932/archive/master.zip)





### Source Code

```
/*
 *Program Name : UserInput Class
 *Description : User Input Class
 *Author	 : Prakash Yogarajah
 */
import java.io.*;
/*
 *UserInput class helps to get userinput from user
 */
public class UserInput
{
     /*
	 *Readln method -> Reads user input
	 *returns the input string
	 */
	public String readln()
	{
		String input = "";
		//reader as BufferedReader
		BufferedReader reader;
		reader = new BufferedReader(new InputStreamReader(System.in));
		try
		{
			input = reader.readLine();
		}
		catch(IOException io)
		{
			System.out.println("Error reading!");
		}
		return input;
	}
	/*
	 *This example may look silly, but a beginner will learn lot new
	 *things from this..
	 */
	public static void main(String[] args)
	{
		UserInput input = new UserInput();
		System.out.println("Sue: What is your name?");
		System.out.print("Jhon: ");
		String name = input.readln();
		System.out.println("Sue: How old are you? if u dont mind.");
		System.out.print("Jhon: ");
		String age = input.readln();
		System.out.println("\n\nSue: Nice to meet you, " + name);
		System.out.println("Jhon: You too!");
		System.out.println("Sue : Are you sure, you are " + age + " years old");
	}
}
```

