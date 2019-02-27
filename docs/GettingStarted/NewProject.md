# Step-by-step tutorial: Create a new project

Let's walk through how to create some `dotnet try`-powered documentation from scratch. 

1. Go to the terminal and create a folder called `MyDocProject`.

2. Create a file called `doc.md`. Inside that file, add some text and a code fence:

<pre>
    <code>
# My code sample:

```cs ./MyConsoleApp/Program.cs --project ./MyConsoleApp/MyConsoleApp.csproj
```
    </code>
</pre>

3. Inside the `MyDocProject` folder, create a subfolder called `MyConsoleApp`, navigate into that folder in your terminal, and run the following command:

    ```console
    > dotnet new console`
    ```

    This will create a console app with the files `MyDocProject.csproj` and `Program.cs`.

4. Now, navigate back to the `MyDocProject` folder and run the following command:

    ```console
    > dotnet try
    ```

    If you want to run this command from elsewhere, you can also pass the path as an argument, like this: 
    
    ```console
    > dotnet try /path/to/your/project/folder
    ```

**Tada!** You have created your first C# interactive developer experience. You should now be able to run your console app and see the result in the browser.  

As you might have noticed, you see the full `Program.cs` file. But suppose you'd like to show your user only `Console.WriteLine("Hello World!");`? The next step in the tutorial will show you how to do that.

**[< Quickstart](./QuickStart.md) &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [ Define regions >](./Regions.md)**