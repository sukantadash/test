Step-by-Step: Use 3scale-cms Native Binary from GitHub
🔹 1. Visit the GitHub Releases Page
Go to:
👉 https://github.com/FwMotion/3scale-cms/releases

Look for the version v2.0.1.

🔹 2. Download the Native Executable
Under the release assets for v2.0.1, look for a file like:

3scale-cms-v2.0.1-native-linux-x86_64

Click to download it or use wget:

bash
Copy
Edit
wget https://github.com/FwMotion/3scale-cms/releases/download/v2.0.1/3scale-cms-v2.0.1-native-linux-x86_64
🔹 3. Make It Executable
Once downloaded, mark it as executable:

bash
Copy
Edit
chmod +x 3scale-cms-v2.0.1-native-linux-x86_64
You can rename or move it to a directory in your $PATH for easier usage:

bash
Copy
Edit
sudo mv 3scale-cms-v2.0.1-native-linux-x86_64 /usr/local/bin/3scale-cms
🔹 4. Test the CLI
Now test it:

bash
Copy
Edit
3scale-cms --help
You should see the CLI help output confirming it's working.

✅ You're Ready!
You can now use it to interact with the 3scale Developer Portal CMS directly, e.g.:

bash
Copy
Edit
3scale-cms pull --provider-key=<your-key> --destination=./portal-backup
