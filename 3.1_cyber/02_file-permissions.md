# Understanding File Permissions

## Task 1 --- Create a File

Run:

    touch secret.txt
    ls -l secret.txt

### Screenshot

<img width="613" height="50" alt="image" src="https://github.com/user-attachments/assets/91139f39-e7bd-4f3c-a04b-47289ba6bb6a" />


### Questions

1.  Who owns the file?
2.  What are the default permissions?

### Reflection

Why is file ownership important in Linux systems?

------------------------------------------------------------------------

## Task 2 --- Restrict File Permissions

Run:

    chmod 600 secret.txt
    ls -l secret.txt

### Screenshot

<img width="546" height="55" alt="image" src="https://github.com/user-attachments/assets/34873bed-c489-4118-b50a-11d2d50d1cfa" />


### Questions

1.  Who can read the file now?
2.  Who cannot access it?


------------------------------------------------------------------------

## Task 3 --- Open Permissions (Security Risk)

Run:

    chmod 777 secret.txt
    ls -l secret.txt

### Screenshot

<img width="551" height="52" alt="image" src="https://github.com/user-attachments/assets/4f95b810-e832-4a7d-b260-3e4ed6e7e181" />


### Questions

1.  Who can access the file now?
2.  Why might this configuration be dangerous?

