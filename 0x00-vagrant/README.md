# Setting Up 0x00-vagrant Directory and Ubuntu VM

In this step, you'll create a new directory named `0x00-vagrant` inside the `zero_day` repository. You'll also create a `README.md` file with information about the `uname` command when run without any options. Let's get started!

## Creating the 0x00-vagrant Directory and README.md File

1. **Inside the `zero_day` Repository**:
   - Open your terminal.
   - Navigate to your `zero_day` repository using the appropriate commands.
   - Create a new directory named `0x00-vagrant` using the following command:
     ```bash
     mkdir 0x00-vagrant
     ```
   - Navigate into the new directory:
     ```bash
     cd 0x00-vagrant
     ```
   - Create a `README.md` file using your preferred command-line editor. You can use commands like `emacs README.md` or `nano README.md`.

2. **Content for README.md**:
   In the `README.md` file you just created, type the answer to the following question:

   > What does the command `uname` print when you run it without any option?

   Save the file after entering your answer.

## SSH into Your Ubuntu VM and Retrieve Information

1. **SSH into Your VM**:
   - Open your terminal.
   - Use the `ssh` command to connect to your Ubuntu VM. Replace `username` with your actual username and `IP_address` with your VM's IP address.
     ```bash
     ssh username@IP_address
     ```

2. **Run the `uname` Command**:
   - Once connected to your VM, run the `uname` command without any options:
     ```bash
     uname
     ```
   - Note down the output.

3. **Update the File**:
   - Return to the terminal on your local machine.
   - Navigate to the `0x00-vagrant` directory within the `zero_day` repository.
   - Create a new file named `0-hello_ubuntu.md` using your preferred command-line editor.

4. **Content for 0-hello_ubuntu.md**:
   In the `0-hello_ubuntu.md` file, type the output of the `uname` command that you observed when running it on your Ubuntu VM.

## Push to GitHub

1. **Add, Commit, and Push**:
   - In the terminal, navigate to the `0x00-vagrant` directory.
   - Use the following commands to add, commit, and push your changes to GitHub:
     ```bash
     git add 0-hello_ubuntu.md
     git commit -m "Add output of uname command"
     git push origin master
     ```

2. **Check GitHub**:
   - Visit your GitHub repository (`zero_day`) and navigate to the `0x00-vagrant` directory. You should see the `0-hello_ubuntu.md` file with the updated content.

Congratulations! 
