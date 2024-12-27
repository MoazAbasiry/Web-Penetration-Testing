# Web-Penetration-Testing
OwaspJuiceShop_Project




## 1. Enumeration to Find Admin Path

![Screenshot 2024-12-27 203330](https://github.com/user-attachments/assets/a89661fd-a4fd-4305-b488-a2169c95bd55)


*Using Ffuf (Fuzzing tool) to find hidden URL's that can make me access the website as an admin*


![Screenshot 2024-12-27 203346](https://github.com/user-attachments/assets/3869c20c-3206-4043-9f6a-3544ed10103d)


*The output of searching process with filter (grip admin) to make search easier*


![Screenshot 2024-12-27 175624](https://github.com/user-attachments/assets/299e9b0e-3b01-4bc8-968a-625709c9f870)


*Discovering any bug in source code using debugger in inspect (Devolper mode) and searching for any path to access as an admin*


![Screenshot 2024-12-27 175455](https://github.com/user-attachments/assets/0f3c01d7-4295-40ef-a3b4-d759935282ea)


*Use localhost:3000/Administration after finding it and access in admin control page*


## 2. Brute Force on Admin Credentials

![1](https://github.com/user-attachments/assets/972a378b-62d2-41ea-ad86-154b704871c9)


*First try to login with valid email (admin@juice-sh.op) and wrong password*


![2](https://github.com/user-attachments/assets/54847e6e-64e9-4b83-b506-449ce2dd29e2)


*Use burpsuite  to get log in traffic by proxy*


![3](https://github.com/user-attachments/assets/b38e909f-3539-4831-9daa-e5504818f409)


*Open intruder to mark the password the inpute we want to make payload on it*


![4](https://github.com/user-attachments/assets/3b738d2e-255e-403e-8606-a377fc00c52d)


*Put in the payload par the passwords you want to use it in payload*


![5](https://github.com/user-attachments/assets/989f567f-c1bd-49dc-b110-b38b917d1acd)


*The payload with large path response is the right password*


![6](https://github.com/user-attachments/assets/c67d7e96-dc57-467b-ae65-2ca642e27365)


*Login with this password and you will get all admin control*


## 3. XSS in Product Search

![1](https://github.com/user-attachments/assets/68392522-d557-49ee-8779-dc79a43c3c04)


*Made unvalidated redirect (whitelist) to bitcoin site*


![2](https://github.com/user-attachments/assets/1e43a935-a905-4565-bc57-be5d3e45a35e)


*Used xss on search bar to send alert*


![3](https://github.com/user-attachments/assets/9f9f7508-3d8d-441b-80ea-99f8ea1d0610)


*Used script to steal cookies from user*


![4](https://github.com/user-attachments/assets/47561287-c7e4-4280-9030-d635cceefc08)


*Redirect user by xss to soundcloud song*

