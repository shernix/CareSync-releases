<p align="center">
  <img src="assets/caresync-logo.png" width="128" alt="CareSync logo">
</p>

<h1 align="center">CareSync</h1>

<p align="center">
  <b>Patient management for your practice.</b><br>
  Private, works offline, and keeps every record encrypted on your own computer.
</p>

<p align="center">
  <a href="https://github.com/shernix/CareSync-releases/releases/latest"><img alt="Latest version" src="https://img.shields.io/github/v/release/shernix/CareSync-releases?label=latest%20version&style=flat-square&color=6c63d9"></a>
  <img alt="macOS and Windows" src="https://img.shields.io/badge/runs%20on-macOS%20%7C%20Windows-1fc98e?style=flat-square">
  <img alt="Works offline" src="https://img.shields.io/badge/works-offline-3d8bd9?style=flat-square">
</p>

<br>

<p align="center">
  <a href="https://github.com/shernix/CareSync-releases/releases/latest/download/CareSync-macOS.dmg"><img alt="Download for Mac" src="assets/download-mac.svg" width="280"></a>
  &nbsp;&nbsp;
  <a href="https://github.com/shernix/CareSync-releases/releases/latest/download/CareSync-Windows-Setup.exe"><img alt="Download for Windows" src="assets/download-windows.svg" width="280"></a>
</p>

<p align="center">
  <sub>
    Mac: Apple Silicon and Intel, macOS 10.15 or newer &nbsp;·&nbsp; Windows 10 or 11, 64-bit
    <br>
    <a href="https://github.com/shernix/CareSync-releases/releases">All versions and what's new</a>
  </sub>
</p>

<br>

## Install in three steps

| | Mac | Windows |
| :---: | --- | --- |
| **1** | Click **Download for Mac** and open the `CareSync-macOS.dmg` file. | Click **Download for Windows** and run `CareSync-Windows-Setup.exe`. |
| **2** | Drag **CareSync** into the **Applications** folder. | Click through the installer. No administrator rights are needed. |
| **3** | Open CareSync from **Applications**, then approve it once (see below). | If Windows shows a warning, approve it once (see below). |

<details>
<summary><b>Mac: "Apple could not verify CareSync…"</b></summary>
<br>

CareSync isn't signed with a paid Apple developer certificate yet, so macOS asks you to approve it the first time:

1. Click **Done** on the warning.
2. Open **System Settings → Privacy & Security** and scroll down.
3. Click **Open Anyway** next to the CareSync message, then confirm with your Mac password.

You only do this once. Updates installed from inside CareSync don't ask again.
</details>

<details>
<summary><b>Windows: "Windows protected your PC"</b></summary>
<br>

SmartScreen shows this for apps without a paid code-signing certificate. Click **More info**, then **Run anyway**. You only do this once.

If your computer doesn't have Microsoft Edge WebView2 (it's built into Windows 11), the installer adds it, which needs an internet connection.
</details>

## Get started

1. **Create the first account.** The first screen asks for a username, email and password. The first account is the practice's **administrator**.
2. **Add the rest of the team.** Each person starts CareSync on the same computer, opens the **Request account** tab, fills it in and clicks **Send request**. The administrator approves each request on the **Users** page, and can make other people administrators too.
3. **Set up the practice.** Administrators add the practice's doctors on the **Providers** page, and review what CareSync tracks on the **Compliance Rules** page, including the preventive care rules, which start switched off.
4. **Add patients.** New patients are visible only to you. To share one, open the patient and choose **All users** or **Specific users** in its **Access** section.
5. **Keep your password safe.** CareSync works offline, so there is no email reset. If you forget your password, an administrator can set a new one for you.

## Try it with sample patients

Want to see CareSync with data before adding your own? Download **[CareSync-Sample-Patients.json](https://github.com/shernix/CareSync-releases/releases/latest/download/CareSync-Sample-Patients.json)**: 100 made-up patients and 4 providers, with diagnoses, medications and two years of visits, labs and screenings.

1. In CareSync, open **Data & Backups** (the gear icon, top right).
2. Click **Import from file** and choose the downloaded file.
3. Choose **Add to current data**, so anything you already have is kept.

Everyone in the file is fictional. Use it on a test account or a computer without real patients, so made-up records don't mix with real ones.

## Updates

Open the user menu (the person icon, top right) and choose **Check for updates**. If a new version is available, click **Update now**. CareSync saves a copy of your data, installs the update and restarts.

CareSync only goes online when you check for updates. It never sends your data anywhere.

## Your data stays yours

- **On your computer only.** Patient records are stored locally, never in the cloud.
- **Encrypted.** The database is encrypted, with its key kept in your Mac's Keychain or Windows Credential Manager.
- **Private per user.** Each person logs in and sees only the patients they own or that were shared with them.
- **Backups when you want them.** **Data & Backups** saves your patients to Excel or JSON, and every export is recorded.

## Questions

<details>
<summary><b>My Mac asks for my password after an update. Is that normal?</b></summary>
<br>

Yes. macOS checks that the updated CareSync may still use its encryption key. Enter the password you use to log in to your **Mac** (not your CareSync password) and click **Always Allow**.
</details>

<details>
<summary><b>Do I need the internet?</b></summary>
<br>

Only to download CareSync and to check for updates. Everything else works offline.
</details>

<details>
<summary><b>Where is my data stored?</b></summary>
<br>

- **Mac:** `~/Library/Application Support/com.caresync/`
- **Windows:** `%APPDATA%\com.caresync\`

The `backups` folder there holds automatic encrypted copies, made before every import and update.
</details>

<details>
<summary><b>How do I move to a new computer?</b></summary>
<br>

On the old computer, use **Data & Backups → Save as Excel** or **Save as JSON**. Install CareSync on the new computer, create your account, then use **Data & Backups → Import from file**.

Accounts aren't part of backups, so each person creates their account again. On a Mac, moving everything with Migration Assistant also works.
</details>

<details>
<summary><b>I forgot my password.</b></summary>
<br>

Ask an administrator. On the **Users** page they can set a new password for your account, and you keep all your patients. You can then change it to one only you know in **Account settings**.

If the only administrator forgets their password, nobody can reset it, because CareSync has no online account system. Making a second person an administrator avoids this.
</details>
