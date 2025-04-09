Create a Separate User Account for Daily Use (Optional but Recommended):**

If you only have one user account that you created during installation, it likely has `sudo` privileges. For enhanced security, consider creating a separate user account for your everyday tasks that doesn't have `sudo` access.

* **Explanation:** This limits the potential damage if your regular user account is compromised. An attacker would have fewer privileges to exploit.
* **How to create a new user:**
    * Open the Terminal.
    * Type the following command (replace `newusername` with your desired username):

    ```bash
    sudo adduser newusername
    ```

    * You'll be prompted to set a password for the new user and provide some optional information.
    * To add this new user to the `sudo` group (if you need to grant them administrative privileges occasionally), type:

    ```bash
    sudo usermod -aG sudo newusername
    ```

    * You can then log out of your current account and log in with the new user account for your daily activities.
