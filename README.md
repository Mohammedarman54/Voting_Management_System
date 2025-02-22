# Voter and Candidate Management System  

## 📌 Introduction  
The **Voter and Candidate Management System** is a console-based C program that allows users to **add, delete, search, and display** voters and candidates using **linked lists**. The system ensures **age eligibility criteria** for both voters and candidates.  

---  

## 📂 Features  
✅ Add new voters (Minimum age: **18 years**)  
✅ Delete voters by name, age, and ID  
✅ Add new candidates (Minimum age: **35 years**)  
✅ Delete candidates by name  
✅ Search for a voter by **name and ID**  
✅ Search for a candidate by **name**  
✅ Display all registered **voters and candidates**  
✅ Ensures **no duplicate voter IDs**  

---  

## 🛠️ Requirements  
- **Operating System**: Windows, Linux, or macOS  
- **Compiler**: GCC (MinGW for Windows)  
- **Editor**: VS Code (Recommended)  

---  

## ⚙️ Installation & Setup  

### **1️⃣ Install GCC Compiler (If Not Installed)**  
- **Windows**: Install MinGW from [SourceForge](https://sourceforge.net/projects/mingw-w64/)  
- **Linux (Ubuntu/Debian)**:  
  ```sh  
  sudo apt install gcc  
  ```  
- **Mac (Homebrew)**:  
  ```sh  
  brew install gcc  
  ```  

### **2️⃣ Clone or Download the Project**  
```sh  
git clone https://github.com/your-username/voter-management.git  
cd voter-management  
```  

### **3️⃣ Compile the C Program**  
```sh  
gcc main.c -o voter_management  
```  

### **4️⃣ Run the Program**  
```sh  
./voter_management   # Linux/macOS  
voter_management.exe  # Windows  
```  

---  

## 🖥️ Usage  
Once the program starts, you will see a menu like this:  

```
Enter your choice  
1. Add new voters  
2. Delete voters  
3. Add new candidates  
4. Delete candidates  
5. Display voters  
6. Display candidates  
7. Search Voter  
8. Search candidate  
9. Exit  
```  

### **Example Operations**  

#### ➤ **Adding a Voter**  
```
Enter your choice: 1  
Enter the name of the voter: John  
Enter the ID: 101  
Enter the age of the voter: 25  
```  
✅ **Output:** *Voter added successfully*  

#### ➤ **Searching for a Voter**  
```
Enter your choice: 7  
Enter the voter to be searched: John  
Enter the ID of the voter: 101  
```  
✅ **Output:** *Voter found: John, ID: 101*  

#### ➤ **Deleting a Voter**  
```
Enter your choice: 2  
Enter voter name to delete: John  
Enter the voter age: 25  
Enter the ID: 101  
```  
✅ **Output:** *Deleted voter is: John of age: 25*  

---  

## 🛠️ Functions Used  
| Function | Purpose |  
|----------|---------|  
| `voterinsertion(Voter*, Voter*, int, int)` | Inserts a new voter into the linked list |  
| `voterdeletion(Voter*, char*, int, int)` | Deletes a voter by name, age, and ID |  
| `candidateinsertion(Candidate*, Candidate*)` | Inserts a new candidate into the linked list |  
| `candidatedeletion(Candidate*, char*)` | Deletes a candidate by name |  
| `searchvoter(Voter*, char*, int)` | Searches for a voter by name and ID |  
| `searchcandidate(Candidate*, char*)` | Searches for a candidate by name |  
| `displayvoter(Voter*)` | Displays all registered voters |  
| `displaycandidate(Candidate*)` | Displays all registered candidates |  

---  

## 🔥 Test Cases  

| **Scenario** | **Input** | **Expected Output** |  
|-------------|----------|-------------------|  
| **Add valid voter** | `1 → John → 101 → 25` | `"Voter added successfully"` |  
| **Add underage voter** | `1 → Bob → 102 → 16` | `"Voter not eligible to vote"` |  
| **Add valid candidate** | `3 → Alice → 40` | `"Candidate added successfully"` |  
| **Add underage candidate** | `3 → Mike → 30` | `"The candidate is not eligible"` |  
| **Search existing voter** | `7 → John → 101` | `"Voter found: John, ID: 101"` |  
| **Search non-existing voter** | `7 → David → 105` | `"Voter not found"` |  
| **Delete existing voter** | `2 → John → 25 → 101` | `"Deleted voter is: John of age: 25"` |  
| **Delete non-existing voter** | `2 → David → 22 → 105` | `"Searched voter is not present"` |  
| **Delete existing candidate** | `4 → Alice` | `"Deleted candidate is: Alice"` |  
| **Delete non-existing candidate** | `4 → Sarah` | `"Searched candidate is not present"` |  

---  

## 📜 License  
This project is **open-source** and free to use under the **MIT License**.  

---  

## 🤝 Contributing  
Feel free to **fork** this repository and submit **pull requests** for improvements.  

---  

## 📩 Contact  
**Developer:** Mohammed Arman Ali  
📧 **Email:** mohammedarmanali1934@gmail.com  
🔗 **GitHub:** [Mohammedarman54](https://github.com/Mohammedarman54)  
🔗 **LinkedIn:** [Mohammed Arman Ali](https://www.linkedin.com/in/mohammed-arman-ali-b58829258/)
