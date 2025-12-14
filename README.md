## Youtube Video Link: <br>
https://youtu.be/Ke8OaP_klJw?si=Rz4XebJxZ0d_v49M

# Merging-of-Branches-using-Git-Commands

## Step 1 — Create a new SSH key <br>
ssh-keygen -t ed25519 -C "your_email@example.com"<br>
press Enter<br><br>

## Step 2 — Start SSH agent and add the key<br>
eval "$(ssh-agent -s)"<br>
ssh-add ~/.ssh/id_ed25519<br><br>

## Step 3 — Add the SSH key to GitHub<br>
Show the public key:<br>
cat ~/.ssh/id_ed25519.pub<br><br>

Copy the entire output (starts with ssh-ed25519).<br>

Go to GitHub → Settings → SSH and GPG keys → New SSH Key.<br>

Paste your key and save.<br>

## Git CLI<br>
nano .gitignore -> Create the file and add the lines automatically<br>

Press Ctrl + O → Enter → Ctrl + X to save and exit<br>

ls -a<br>

git status -> current status of branch<br>

git init -> Think of it like turning a regular folder into a Git folder.<br>

After this, Git can track changes, commit versions, create branches, and so on.<br>

git add . -> add files ready to commit (stagged area)<br>

git restore --staged . -> restore files from stage to unstage<br>

git branch <branch_name> -> creating branch<br>

git checkout <branch_name> -> switching between branches<br>

Before Commit, check first<br>

git config --global --list<br>

then<br>

git config --global user.name "Nadir Abbas"<br>
git config --global user.email "nadir@example.com"<br>

git commit -m "Add basics module" -> give change the name<br>

git push -u origin branch1_basics -> sends your branch/files/changes to GitHub<br>

Clone after merging<br>

git clone -> only clone main branch<br>

git branch -r -> to see remote branches<br>

git checkout -b branch_1 origin/branch_1<br>



<br>
Each branch adds one part of the system.<br>
In the end, merging them will show how different parts combine into one working project.<br>

## Branch 1 — Basic Input/Output + Conditions + Loops<br>

Implement/Add Functions<br>

void inputMarks(int marks[], int n);<br>

int getTotal(int marks[], int n);<br>

float getAverage(int marks[], int n);<br>

void showPassFail(int marks[], int n);<br>

## Branch 2 — Functions + Searching in Arrays<br>

Implement/Add functions:<br>

int getHighest(int arr[], int n)<br>

int getLowest(int arr[], int n)<br>

float getAverage(int arr[], int n)<br>

Add a search function:<br>
int searchStudent(string names[], int n, string key)<br>

## Branch 3 — Pointers + Swapping + Pass-by-Reference<br>

Implement/Add functions:<br>

void swapNums(int *a, int *b);<br>

void increaseMarks(int *m);<br>

## Branch 4 — Structures + Arrays of Structures<br>

Implement/Add<br>

Create a structure:<br>

struct Student {<br>
    string name;<br>
    int roll;<br>
    float marks;<br>
};<br>


void inputStudent(Student &s);<br>

void printStudent(const Student &s);<br>

float classAverage(Student s[], int n);<br>


## Final Merge — Combined Project<br>

This will contain<br>
1. Structure for student<br>

2. Functions from branch 2<br>

3. Pointer-based update from branch 3<br>

4. A menu system from branch 1<br>
