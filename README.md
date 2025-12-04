# domashnoprivladov

# Mini Library System (C++)

Това е малък проект за библиотечна система, написан на C++. Включва няколко класа: Author, Book, Member, Loan и Library. Примерната програма тества различните функции.

---

##  Как се компилира

Примерна команда за компилация:


g++ -std=gnu++17 -Wall -Wextra -O2 -o library main.cpp Author.cpp Book.cpp Member.cpp Loan.cpp Library.cpp


---

##  Кратко описание на класовете

### **Author**
- name  
- birthYear  
- валидация за година  
- `to_string()`  

### **Book**
- title  
- author (обект Author)  
- year  
- price  
- isbn  
- статичен `totalBooks`  
- Rule of 5 (копиране/преместване)  
- `to_string()`  

### **Member**
- name  
- memberId  
- yearJoined  
- валидиране на ID  
- `to_string()`  

### **Loan**
- isbn  
- memberId  
- startDate  
- dueDate  
- returned  
- проверка дали е просрочена  
- `markReturned()`  

### **Library**
- списък от книги, членове и заеми  
- добавяне на книга и член  
- проверка дали дадена книга е налична  
- създаване и връщане на заем  
- търсене по автор  
- `to_string()`  

---

##  Примерен изход


Library info:
Books: 2
Members: 1
Active loans: 1

Loan created.
Available ISBN-001? false
Available ISBN-001? true
Pod igoto (1894) - 25.50 лв.
Nema zemya (1900) - 18.90 лв.

---

Author: Ivan Vazov
Book: Pod igoto
Member: Petar Petrov
Loan: ISBN-001 → M001 (2025-11-03 → 2025-11-17)


---

Ако искаш, мога да ти направя README-то по-кратко, на английски, или да добавя секции като „Структура на проекта“.



