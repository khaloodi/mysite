## Run application
    python3 manage.py runserver

<br/>

## Steps To Apply Migrations (e.g. creating tables) 
    python3 manage.py migrate

### 1. Tell Django you have made changes to DB model
    python3 manage.py makemigrations <app name>
    python3 manage.py makemigrations food

### >>
![](0001.png)

### 2. Create the actual table referenced above
    python3 manage.py sqlmigrate food 0001 
    # notice the 0001 was provided by django

### >>    
![](successful_table_creation.png)

### 3. Apply migrations
    python3 manage.py migrate

### >>
![](last_step.png)



