---

# Whisper Live Transcription 🎤
An easy guide for your PC to transcribe any audio **free and in real-time** using Google Colab

---

### Step 1: Enable Your PC's "Internal Sound"

This allows the program to "listen" to the audio from your videos, calls, or games.

1.  On your taskbar (bottom-right), right-click the **Sound** icon.
2.  Choose **"Sound settings"** and then **"More sound settings"**.
3.  A new window will open. Go to the **"Recording"** tab.
4.  If you don't see **"Stereo Mix"**, right-click on an empty space and check **"Show Disabled Devices"**.
5.  Now, right-click on **"Stereo Mix"** and select **"Enable"**.
6.  Click **Accept** to save.

### Step 2: Set Up a Chrome Profile

We'll create a dedicated Chrome profile for this so you don't change your main browser's settings.

**First, create the profile:**
1.  In Chrome, click your **profile icon** (top-right).
2.  Click **"+ Add Chrome profile"**.
3.  Select **"Continue without an account"**.
4.  Give it a name (e.g., `record`) and click **"Done"**.

**Now, configure the microphone for this profile:**
1.  In your new `record` profile, go to the three-dot menu (`⋮`) and open **"Settings"**.
2.  Find and open **"Site Settings"**.
3.  Click on **"Microphone"**.
4.  At the top, where you choose the microphone, select **"Stereo Mix"**.

**Finally, keep the necessary sites active:**
1.  In Settings, go to the **Performance** section.
2.  In the "Always keep these sites active" area, click **Add**.
3.  Add the following sites one by one:
    *   `colab.research.google.com`
    *   `[*.]gradio.live`

### Step 3: Install an Extension

This prevents the transcription from stopping if you switch to another window.

1.  Install [**Always Active Window**](https://chromewebstore.google.com/detail/always-active-window-alwa/ehllkhjndgnlokhomdlhgbineffifcbj) from the Chrome Web Store.
2.  Click the **puzzle icon** (`🧩`) for extensions (top-right).
3.  Find the extension, click the three-dot menu (`⋮`) next to it, and choose **"Options"**.
4.  In the text box, paste the following (all on one line):
    ```
    colab.research.google.com, *.gradio.live
    ```
5.  Save the changes with the **Save Options** button.

### Step 4: Start Transcribing!

Now for the magic part.

1.  Open this link in your `record` Chrome profile:
    > **[Start Live Transcription](https://colab.research.google.com/drive/1H8-Uc8O08d3VkBzLTQzJGgLZPkwAoimW?usp=sharing)**

2.  In the notebook's top menu, go to **"Runtime"** and click **"Run all"**.

3.  **Permissions:** It will ask you to **sign in** with your Google account and then **grant permission to use Google Drive**. Accept both prompts.

4.  **Wait a moment.** The program is setting up. At the end, you will see a **blue link** ending in `.gradio.live`.

5.  **Done!** Click that link. A new tab will open where you'll see a real-time text transcription of your PC's audio.

---

### How to Stop Everything

When you're finished, go back to the Google Colab tab, open the **"Runtime"** menu, and select **"Disconnect and delete runtime"**.

---

### About Free Usage and Paid Options

The **free** tier of Google Colab is great, but it has a weekly usage limit (usually around **3-5 hours**). If you exceed it, your session may be terminated.

**If you need it more often or for longer periods:**

I recommend buying "compute units" to avoid these limits.

-   You can buy **100 compute units** (valid for 3 months) for **$9.99** on the "Pay-As-You-Go" plan here: [**Buy Colab Compute Units**](https://colab.research.google.com/signup)
-   **100 units** ≈ **55 hours of transcription**.

> For more details on performance and pricing, you can check this [reference article](https://mccormickml.com/2024/04/23/colab-gpus-features-and-pricing/).

**How to check your remaining units?**

In Google Colab, look in the top-right corner of the page. Find the 'Connect' button or the RAM/Disk display. Click the little down arrow (⬇️) next to it, and then choose 'View resources', here you'll see your available units.
