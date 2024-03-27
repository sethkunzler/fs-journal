# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > Namespaces are used to organize import/exports and avoid name conflicts

02. What is the difference between a `class` and an `interface`?

  > interfaces only contain a definition where as classes have both a definition and an implementation.

03. What is the method that returns an instance of a class, yet it has no return type?

  > a singleton class

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > 'abstract' is the access modifier

06. In the Car example what is `string` an indication of?

  > 'string' is an indication of a data type 

07. In the Car example what is `abstract` preventing?

  > abstract is preventing changes to the class from outside the class.

08. In a SQL table, what is the difference between information in a row and information in a column?

  > the information in the row would be the information in a collective object, where information in each collumn describes a specific aspect
  i.e. row --> ('Mazda', 'Miata', $8000, 'red')
  i.e. column --> ('Make', 'Mazda', 'Honda', 'Ford')

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  >```c# 
    CREATE TABLE characters(
      id INT NOT NULL PRIMARY KEY AUTO_INCRAMENT,
      name VARCHAR(255) NOT NULL,
      age VARCHAR(255) NOT NULL,
      description VARCHAR(255) NOT NULL
    );
  ```

10. In SQL how can you query more than a single table? Provide an example.

  > by using a join operation 
  ```cs 
  SELECT table1.collumn1, table2.collumn2 FROM table1, table2 WHERE table1.column1 = table2.collumn2
  ```
