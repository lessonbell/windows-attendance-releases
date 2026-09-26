<p align="center">
  <img src="https://avatars.githubusercontent.com/u/334188139?v=4" width="72" alt="LessonBell logo">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/lessonbell/.github/main/assets/lessonbell-banner.svg" width="100%" alt="LessonBell — Official apps and downloads">
</p>

<h1 align="center">Windows Attendance Assistant</h1>

<p align="center">
  <strong>Scan. Confirm. Carry on.</strong><br>
  QR attendance for your education centre's reception desk.
</p>

<p align="center">
  <a href="https://github.com/lessonbell/windows-attendance-releases/releases/latest/download/LessonBell.AttendanceScanner-win-stable-Portable.zip"><strong>Download for Windows</strong></a>
  &nbsp; · &nbsp;
  <a href="#quick-start">Quick start</a>
  &nbsp; · &nbsp;
  <a href="#requirements">Requirements</a>
  &nbsp; · &nbsp;
  <a href="#help">Help</a>
</p>

> **Version 1.1.1 is available.** Download the portable ZIP, extract the whole folder and open `LessonBellAttendance.exe`.

## A simple tool for a busy front desk

The LessonBell Windows Attendance Assistant reads QR codes from a selected USB scanner and records attendance in your centre's LessonBell account. It shows the result on screen and plays a distinct success or failure sound.

- **Portable:** extract the complete ZIP and open the app.
- **Focused:** reads only the selected serial scanner; it does not monitor keyboard input.
- **Clear feedback:** attendance results, recent scans and separate success and failure sounds.
- **Flexible alerts:** adjust volume, mute sound and choose whether to show desktop notifications.
- **Out of the way:** minimise to the system tray and reopen from the tray icon.

## Downloads

**[Download the latest Portable ZIP →](https://github.com/lessonbell/windows-attendance-releases/releases/latest/download/LessonBell.AttendanceScanner-win-stable-Portable.zip)**

Read the **[latest release notes](https://github.com/lessonbell/windows-attendance-releases/releases/latest)**. `SHA256SUMS.txt` on the release page can verify download integrity; it is not a Windows publisher certificate.

Download `LessonBell.AttendanceScanner-win-stable-Portable.zip` from its **Assets** section. GitHub's **Source code (zip)** and **Source code (tar.gz)** links are not the app.

## Requirements

| Item | Supported setup |
| --- | --- |
| Windows | Windows 10 22H2 or Windows 11 |
| Architecture | x64 |
| Runtime | .NET Framework 4.8 enabled |
| Scanner | USB virtual serial / CDC mode, not keyboard mode |
| Account | An authorised LessonBell scanner key and branch |
| Connection | Internet access to your centre's LessonBell service |

**Verified scanner:** STAR ASIA BCR12D in USB virtual serial mode.

Other Zebra, Honeywell and USB scanners require model-specific testing before they can be listed as supported. Windows 98, XP, 7, 8, 8.1, 32-bit Windows and Windows on ARM are not supported.

## Quick start

1. Download the **Portable ZIP** from the Releases page.
2. Extract the **entire ZIP** to a writable folder, such as Desktop or Documents.
3. Open `LessonBellAttendance.exe` directly.
4. Ask your centre administrator for the API URL and scanner key from **Developer → API Settings** in LessonBell CMS.
5. Enter those details, validate the connection and select your authorised branch.
6. Select your scanner, which must already be configured for **USB virtual serial mode**, and test a QR code.
7. Keep the app open while scanning. You can minimise it to the system tray.

Keep the full extracted folder together. Do not run the app from inside the ZIP or copy out only the EXE.

## Everyday use

Open the app at the start of each attendance session. Scan a QR code and wait for the result before scanning the next one.

Use the system tray icon to reopen the window or exit the app. Sound volume, mute and desktop notifications are available in Settings.

### If a scan fails

Check the message shown in the app. If a request times out or the internet connection fails, confirm attendance in LessonBell CMS before trying again. The app does not save an offline queue; staff can handle attendance directly in CMS.

## Updates

Version 1.1.1 uses a direct-launch portable ZIP with manual updates. It removes the native update launcher and does not check for updates in the background or replace itself.

1. Choose **Download latest** in Settings or the tray menu, or use the official download link above.
2. Extract the complete new ZIP into a new folder.
3. Exit the old app through its system tray menu, then open the new `LessonBellAttendance.exe`.

Saved connection, branch, scanner, sound and notification settings are preserved on the same computer under the same Windows account. Clicking X only hides the app; use the tray menu to exit completely. Unsaved changes and the current scan list are not carried over.

Users of 1.0.x or 1.1.0 must download the new ZIP manually. The old automatic updater cannot install this direct-ZIP release format. No `current`, `packages` or `Update.exe` is needed.

## Privacy

The app reads only the selected serial scanner and does not capture other keyboard input. Scanner keys are encrypted for the current Windows account using Windows DPAPI. Diagnostic logs do not contain complete scanner keys or raw QR tokens.

Your centre supplies its API URL and scanner key during setup; those details are not included in the public download.

## Help

Contact your centre administrator or your LessonBell support contact. Include your app version, Windows version, scanner model and the error message. The app is not yet Windows code-signed. Windows may show an unknown-publisher warning or block it under some security policies. If blocked, contact support; do not disable security protection.

Do not post scanner keys, QR tokens or student details in public GitHub issues.

---

Official LessonBell app distribution and release notes.

