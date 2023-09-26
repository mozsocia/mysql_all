In MySQL Command Line (mysql), you can list all the databases available on your MySQL server using a simple SQL command. Here's how you can do it:

1. Open a command prompt or terminal window.

2. Log in to MySQL by running the following command and entering your MySQL password when prompted:

   ```
   mysql -u your_username -p
   ```

   Replace `your_username` with your MySQL username.

3. Once you are logged in, you can list all databases by executing the following SQL command:

   ```
   SHOW DATABASES;
   ```

   Here's an example of what it might look like:

   ```sql
   mysql> SHOW DATABASES;
   ```

   This command will display a list of all the databases on the MySQL server.

4. To exit the MySQL Command Line, you can use the following command:

   ```
   exit;
   ```

That's it! You should now see a list of all the databases on your MySQL server using the `SHOW DATABASES;` command in the MySQL Command Line.

------------------
------------------

### import 

You can import data from an SQL file into a MySQL database using the MySQL Command Line or MySQL client. Here are the steps to do it:

**Using MySQL Command Line (mysql):**

1. Open a command prompt or terminal window.

2. Log in to MySQL using your MySQL username and password. You can use the following command:

   ```
   mysql -u your_username -p
   ```

   Replace `your_username` with your MySQL username, and you'll be prompted to enter your MySQL password.

3. Once you are logged in, you can import the SQL file using the following command:

   ```
   mysql -u your_username -p your_database_name < your_sql_file.sql
   ```

   Replace the following:
   - `your_username`: Your MySQL username.
   - `your_database_name`: The name of the database you want to import the SQL file into.
   - `your_sql_file.sql`: The path to the SQL file you want to import.

   Example:

   ```
   mysql -u myuser -p mydatabase < backup.sql
   ```

4. After entering the command, you will be prompted to enter your MySQL password. Once you enter the password, the SQL file will be imported into the specified database.

5. When the import is complete, you can verify the data in your MySQL database.

**Using MySQL Client (mysqlimport):**

Alternatively, you can use the `mysqlimport` command-line utility to import data from an SQL file. Here's how:

1. Open a command prompt or terminal window.

2. Run the `mysqlimport` command with the appropriate options:

   ```
   mysqlimport -u your_username -p --local your_database_name your_sql_file.sql
   ```

   Replace the following:
   - `your_username`: Your MySQL username.
   - `your_database_name`: The name of the database you want to import the SQL file into.
   - `your_sql_file.sql`: The path to the SQL file you want to import.

   Example:

   ```
   mysqlimport -u myuser -p --local mydatabase backup.sql
   ```

3. You will be prompted to enter your MySQL password. Once you enter the password, the SQL file will be imported into the specified database.

4. After the import is complete, you can verify the data in your MySQL database.

That's it! You have successfully imported data from an SQL file into a MySQL database using either the MySQL Command Line or the `mysqlimport` utility.
