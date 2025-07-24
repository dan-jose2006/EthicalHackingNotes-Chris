🔐 Linux Commands & Villain Framework Setup - Detailed Note
🧾 Basic Linux Terminal Commands
Command	Description
mkdir	Used to create a new directory (folder). Example: mkdir testdir will make a directory named testdir.
rmdir	Used to remove an empty directory. Example: rmdir testdir deletes testdir.
touch	Creates a new empty file. Example: touch myfile.txt will make a blank file.
ls	Lists all files and directories in the current location.
cd ..	Moves one step back in the directory path (to parent directory).
ls -lh filename	Lists files with human-readable sizes, used to check file size (can help identify if a file is empty or not).
pwd	Prints the current working directory path.
man ls	Shows the manual (help) page for the ls command. Useful for learning all its options.

💣 Villain Framework (by KeralaHacker)
Villain is a post-exploitation framework used by ethical hackers for compromising Windows systems and setting up reverse shells in penetration tests. It supports multi-client reverse shells over HTTP, HTTPS, or WebSockets.

🛠️ Installation Steps
Clone the repository from GitHub:

bash
Copy
Edit
git clone https://github.com/keralahacker/Villain.git
This command downloads the Villain framework to your system.

git must be pre-installed.

Navigate to the Villain directory:

bash
Copy
Edit
cd Villain
ls
cd Villain enters the folder.

ls confirms files like villain.py and requirements.txt are present.

Install Python requirements:

bash
Copy
Edit
pip3 install -r requirements.txt --break-system-packages
This installs all Python libraries needed to run Villain.

--break-system-packages bypasses pip restrictions on system-wide installs (used in environments like Kali Linux).

If Crypto Library is Missing (Fix Error):

bash
Copy
Edit
pip3 install Crypto --break-system-packages
Crypto is sometimes missing, and Villain won’t run without it.

Run Villain:

bash
Copy
Edit
python3 villain.py
This starts the framework.

You’ll see the Villain dashboard or listener setup options.
