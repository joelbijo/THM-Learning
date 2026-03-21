# Linux Basic Commands

This section covers commonly used Linux commands for searching files, viewing content, and listing directories.

---

## File Search

### find

**Definition:**  
Searches for files and directories based on name, type, size, etc.

**Example:**

```bash
find /home -name "file.txt"
```

**Why it matters:**
Helps locate files quickly in large systems.

---

## Text Search

### grep

**Definition:**
Searches for a specific word or pattern inside a file.

**Example:**

```bash
grep "error" logfile.txt
```

**Why it matters:**
Useful for filtering logs and extracting important information.

---

### grep -R

**Definition:**
Searches for a pattern recursively in a directory.

**Example:**

```bash
grep -R "password" /etc
```

**Why it matters:**
Used to scan entire directories for sensitive data or configurations.

---

## Directory Listing

### ls (with common flags)

**Definition:**
Lists files and directories.

Common Variations:
• ls -a → Shows all files, including hidden files
• ls -la → Detailed view (permissions, size, owner) + hidden files
• ls -A → Shows hidden files, but excludes . and ..

**Example:**

```bash
ls -la
```

**Why it matters:**
Essential for understanding file structure and permissions.

---

## grep vs cat

### cat

**Definition:**
Displays the full content of a file.

**Example:**

```bash
cat file.txt
```

---

**When to use what?**
• Use cat → When you want to view the entire file
• Use grep → When you want to search for specific content inside a file

**Quick Insight:**
cat shows everything, grep helps you find only what matters.

---

# Shell Operators

Shell operators help control how commands are executed in the terminal. They are especially useful for chaining commands and managing output.

---

## & (Run in Background)

**Definition:**  
Runs a command in the background, allowing you to continue using the terminal.

**Example:**

```bash
sleep 10 &
```

**Why it matters:**
Lets you run long tasks without blocking your terminal.

---

## && (AND Operator)

**Definition:**
Runs the second command only if the first command succeeds.

**Example:**

```bash
mkdir test && cd test
```

**Why it matters:**
Ensures commands execute only when the previous one is successful.

---

## > (Overwrite Output)

**Definition:**
Redirects output to a file, overwriting existing content.

**Example:**

```bash
echo "Hello" > file.txt
```

**Why it matters:**
Used to save command output into files.

---

## >> (Append Output)

**Definition:**
Redirects output to a file without deleting existing content.

**Example:**

```bash
echo "World" >> file.txt
```

**Why it matters:**
Useful for logging or adding data without losing previous content.

---

# What I Learned

- Learned how to search for files using `find` in large directory structures
- Understood how to use `grep` to extract specific information from files
- Learned recursive searching with `grep -R` for scanning directories
- Explored different `ls` flags to view hidden files and detailed file information
- Understood the practical difference between `cat` (view everything) and `grep` (search specific content)

- Learned how shell operators control command execution
- Used `&` to run processes in the background
- Used `&&` to chain commands safely based on success
- Learned output redirection using `>` (overwrite) and `>>` (append)

# Common Mistakes

- Using `>` instead of `>>` and accidentally overwriting files
- Running `grep -R` on large directories without filtering (can be slow)
