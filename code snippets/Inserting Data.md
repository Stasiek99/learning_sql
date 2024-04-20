    CREATE TABLE people (
        first_name VARCHAR(20),
        last_name VARCHAR(20),
        age INT
      );


    INSERT INTO people(first_name, last_name, age)
    VALUES ('Tina', 'Belcher', 13);


    INSERT INTO people(age, last_name, first_name)
    VALUES (42, 'Belcher', 'Bob');


    INSERT INTO people(first_name, last_name, age)
    VALUES
        ('Linda', 'Belcher', 45),
        ('Phillip', 'Frond', 38),
        ('Calvin', 'Fischoeder', 70);

   

DROP TABLE people; 

Defining employees table

    CREATE TABLE employees (
        id INT AUTO_INCREMENT,
        first_name VARCHAR(255) NOT NULL,
        last_name VARCHAR(255) NOT NULL,
        middle_name VARCHAR(255),
        age INT NOT NULL,
        current_status VARCHAR(255) NOT NULL DEFAULT 'employed',
        PRIMARY KEY(id)
    );

-- Another way of defining the primary key:


    CREATE TABLE employees (
        id INT AUTO_INCREMENT PRIMARY KEY,
        first_name VARCHAR(255) NOT NULL,
        last_name VARCHAR(255) NOT NULL,
        middle_name VARCHAR(255),
        age INT NOT NULL,
        current_status VARCHAR(255) NOT NULL DEFAULT 'employed'
    );

-- A test INSERT:


    INSERT INTO employees(first_name, last_name, age) 
    VALUES ('Dora', 'Smith', 58);