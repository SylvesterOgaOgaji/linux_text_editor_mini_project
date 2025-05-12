# Mastering Linux Text Editors - A Hands-On Guide to Vim and Nano

## Introduction  
Text editors are indispensable tools in Linux environments, enabling users to create, modify, and manage configuration files, scripts, and documentation. This guide focuses on two widely used editors: **Vim** (Vi Improved) and **Nano**, each catering to different user needs and skill levels.  

### Vim Editor  
Vim is a powerful, modal text editor favored by developers and system administrators for its efficiency and extensibility. Unlike conventional editors, Vim operates in distinct modes:  
- **Normal Mode**: For navigation and command execution (e.g., deleting lines with `dd`).  
- **Insert Mode**: For text input (activated by pressing `i`).  
- **Visual Mode**: For text selection.  

While Vim has a steep learning curve, its keyboard-driven workflow allows for rapid editing once mastered. For example, creating a file named `exercise.txt` is as simple as a few lines of code

## 3. Successful Connection to Remote Ubuntu Server on AWS from Git Bash Local.jpg
![SSH Connection](./img/3.%20Successful%20Connection%20to%20Remote%20Ubuntu%20Server%20on%20AWS%20from%20Git%20Bash%20Local.jpg)

**Command:**
```bash
ssh -i "keytest.pem" ubuntu@ec2-54-226-148-242.compute-1.amazonaws.com
```

### Output:
Welcome to Ubuntu 24.04.2 LTS | System load: 0.0 | Memory usage: 20%
### Explanation:

- -i specifies the identity (PEM key) for authentication.

- Always restrict key permissions:
**Command:**  
```bash
chmod 400 keytest.pem
```
## 4. Creating a new file using vim.jpg
![Vim File Creation](./img/4.%20Creating%20a%20new%20file%20using%20vim.jpg)
**Command:**  
```bash
vim exercise.txt
```
### Output:
Empty file exercise.txt created in home directory.

### Explanation:

- Vim opens in Normal Mode by default.

- Use :wq to save and exit.

## 5. Open a new file with VIM Editor.jpg
![Vim Insert Mode](./img/5.%20Open%20a%20new%20file%20with%20VIM%20Editor.jpg)

**Action:**
Press i to enter Insert Mode.

### Explanation:

- Vim requires mode switching for editing (i = insert, Esc = normal).

- Text can now be added/modified freely.

## 6. Exited insert mode and deleted a character.jpg
![Character Deletion](./img/6.%20Exited%20insert%20mode%20and%20deleted%20a%20charcter.jpg)
**Steps:**

1. Press Esc to exit Insert Mode.

2. Navigate to target character.

3. Press x to delete it.

### Explanation:

- x removes the character under the cursor.

- Undo with u if deleted accidentally.

## 7. Entire line id deleted by pressing dd.jpg
![Line Deletion](./img/7.%20Entire%20line%20id%20deleted%20by%20pressing%20dd.jpg)
**Action:**
Press dd in Normal Mode.

### Output:
Entire line removed instantly.

Explanation:

- dd deletes the current line.

- Combine with numbers (e.g., 3dd) to delete multiple lines.

## 8. Pressing u to undo changes.jpg
![Undo Action](./img/8.%20Pressing%20u%20to%20undo%20changes.jpg)
**Action:**
Press u in Normal Mode.

## Output:
Last action (e.g., deletion) is reverted.

Explanation:

- Vim maintains an undo history for most actions.

- Use Ctrl + r to redo.

## 9. Working with Nano Intro.jpg

This introduction avoids referencing specific images while incorporating key details from the provided content. It sets context, contrasts the two editors, and outlines the project's goals clearly.

### Explanation:

- Nano uses direct editing (no modes).

- Shortcuts like Ctrl + O (save) and Ctrl + X (exit) are displayed at the bottom.

## 10. Opening a file with nano.jpg
![Nano File Creation](./img/10.%20Opening%20a%20file%20with%20nano.jpg)  
**Command:**  
```bash
nano nano_file.txt
```
### Output:
New file nano_file.txt created in home directory.

### Explanation:

- Typo mano shown in image demonstrates common keyboard slip (correct command: nano).

- Nano opens immediately in edit mode with empty buffer for new files.

## 11. Text entered in nano.jpg
![Nano Text Entry](./img/11.%20Text%20entered%20in%20nano.jpg)
**Action:**
**Type directly in Nano interface:**

Hello, this is a Vim hands-on project.
Welcome to darey.io.

### Explanation:

- Nano uses WYSIWYG editing (no modes like Vim).

- Bottom bar shows shortcuts:

  - ^O (Ctrl+O): Save

  - ^X (Ctrl+X): Exit

## 12. Command to opening and existing file.jpg
![Open Existing File](./img/12.%20Command%20to%20opening%20and%20exisiting%20file.jpg)
**Command:**  
```bash
nano nano_file.txt
```
### Output:
Opens existing file with previous content preserved.

### Explanation:

- Nano automatically loads file content if it exists.

- Shows line count (Read 3 lines) in status bar.

## 13. Opening existing file.jpg
![Existing File Edit](./img/13.%20Opening%20existing%20file.jpg)
Interface Features:

1. File name: nano_file.txt (top bar)

2. Content: Pre-existing text from previous edits

3. Shortcuts:

    - Write Out (Ctrl+O): Save changes

    - Read File (Ctrl+R): Insert another file

### Explanation:

- Modified files show asterisk * next to filename until saved.

 - Use Ctrl+G to access full help documentation within Nano.