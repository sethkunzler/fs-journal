# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > Inheritance is when one class takes on the attributes, methods and members of another. In C# it means that  we can do fun things like 
  ``` cs
  <!-- RepoItem.cs -->
  namespace thisProjectName.Models;

  public class RepoItem 
  {
    public int Id { get; set; }
    public DateTime CreatedAt { get; set; }
    public DateTime UpdatedAt { get; set; }
  }

  <!-- Student.cs -->
  namespace thisProjectName.Models;

  public class Student : RepoItem
  {
    <!-- inherits the public property holders ID, CreatedAt, and UpdatedAt -->
    public string FirstName { get; set; }
    public string LastName { get; set; }
  }
  ```

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > members are declared and defined. They are given a level of accessibility so that any other class that inherits will know which members are "private", "public" or otherwise listed.

3. How does ***accessibility*** affect inheritance?

  >Accessibility defines who has access to the different members of a class. public methods and members can be used by any class that inherits the one with this kind of member. private members can only be used within the class itself, and is not inherited into another class.

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > Primary Keys are the unique identifiers for any specific row on a table. a foreign key is when the primary key of another table is referenced

5. What is an ***alias***?

  > A nickname, specifically the name that you give a column of a table when combining two tables with the same named columns. 

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )
  ```

  > 
  ``` cs
  SELECT 
  doctor.*,
  patient.*
  FROM doctors doctor 
  JOIN patients patient ON doctor.id = patient.doctorId
  WHERE doctorId = @DoctorId
  ```
