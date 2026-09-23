# User-Activity-DT-App
Dynatrace App (my.user.activity.monitor) v1.0.5 - Monitors user activity and sends support requests to Email.

## User Activity Monitor

This Dynatrace app monitors user activity and sends support requests directly to Email.

* **App ID:** `my.user.activity.monitor`
* **Version:** `1.0.5`

---

### 📥 Detailed Installation Instructions

Follow these step-by-step instructions to install and configure the User Activity Monitor app in your Dynatrace environment.

#### Step 1: Download the App Package
1. Scroll down to the **Assets** section at the bottom of this release page.
2. Click on the `user-activity-monitor-app-5.0.zip` file to download it to your local computer. *(Do not extract or unzip this file, as Dynatrace requires it in `.zip` format).*

#### Step 2: Navigate to App Management in Dynatrace
1. Open a web browser and log in to your **Dynatrace environment** (e.g., `https://<your-environment-id>.apps.dynatrace.com/`).
2. In the top-left corner of the screen, click the **Dynatrace Launcher** icon (the grid of nine squares).
3. In the launcher search bar, type **"Hub"** or look for the **Hub** interface. Click to open it.
4. In the **Hub** click on **Manage** tab.

#### Step 3: Upload and Install the App
1. Inside the Manage tab screen, locate and click the **Upload App** button.
2. A file selection dialog will appear. Choose the `user-activity-monitor-app-5.0.zip` file you downloaded in Step 1.
3. Dynatrace will begin processing the upload. If you are prompted to approve required scopes/permissions for the app (such as Grail read/write access or AppEngine execution), click **Approve** or **Allow**.
5. Wait a few moments for the installation to finish. The app will now appear in your list of installed apps.

#### Step 4: Whitelist Required External Connections
*The app requires outbound network access to communicate with a third-party service. By default, Dynatrace restricts outbound connections, so you must explicitly allow this domain.*

1. Click the **Dynatrace Launcher** (grid icon in the top-left) again.
2. Search for and open the **Settings** app.
3. In the left-hand navigation menu of the Settings app, scroll down and expand the **General** section.
4. Click on **External requests**.
6. Click the **New host pattern** (or **Add item**) button.
7. In the input field that appears, type exactly: `live2.dreamcast.in`
8. Click the **Save changes** button at the bottom of the screen. *(Note: It may take up to 10 seconds for the networking changes to fully propagate across the environment).*

🎉 **Installation Complete!** You can now launch the **User Activity Monitor** app from your Dynatrace Launcher.
