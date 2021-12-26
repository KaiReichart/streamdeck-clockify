<p align="center">
  <a href="#">
    <img src="resources/readme/GitHubBanner.png" alt="Clockify + Elgato Stream Deck" />
  </a>
</p>

<p align="center">
  <a href="#">
    <img src="https://img.shields.io/badge/macOS-✓-success?logo=apple&style=flat-square&logoColor=white" alt="macOS supported" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Windows-✓-success?logo=windows-95&style=flat-square&logoColor=white" alt="Windows supported" />
  </a>
</p>

___

# Hassle-free time tracking using [Elgato Stream Deck](https://www.elgato.com/en/gaming/stream-deck) and [Clockify](https://clockify.me/)

This is a fork of the awesome [Toggl integration by tobimori](https://github.com/tobimori/streamdeck-toggl), modified to work with clockify instead of toggl.

## ✏️ Setup

Just search for the Action "Clockify" within the Stream Deck app and install it. There is a button called "Clockify" available in section "Custom".

![PropertyInspector](resources/readme/PropertyInspector.png)

* **Title** is a default Stream Deck property available for every button in Stream Deck. You should leave it empty (see Button Label).
* **API Token** is your private API Token you can get from your [Toggl profile](https://track.toggl.com/profile). This Token is handled like a password. ***Don't share it***. Required.
* **Button Label** is used instead of *Title*. If the tracker isn't running, the Label is shown on the button. If the tracker is running the elapsed time is shown additionally. If *Title* is set, it will override *Button Label*.
* **Entry Name** describes the activity you want to report. It is not required but strongly recommended.
* **Workspace** is your workspace you start the time entries in. Required.
* **Project** is the project you want to assign the task to. Leave blank for no project. New projects can be added in Toggl.
* **Billable** sets Toggl's billable flag (for Toggl paid plans only).

![StreamDeckScreenshot](resources/readme/StreamDeckScreenshot.png)

Just press any Clockify Button to start tracking time. The button should indicate tracking by turning red and showing the current tracking time (if no *Title* is set). The status of the button is defined by workspace, project and entry name. If you setup two identical buttons (even on different Stream Deck profiles), both button indicate the same. If you start or stop your timer using the Clockify app (web, desktop, mobile) Clockify for Stream Deck will follow by changing the status.

## 📞 Help

Please use GitHub Issues for reporting bugs and requesting new features.

## 📄 License

streamdeck-toggl is licensed under the [MIT License](LICENSE).

## Known Issues

* Changing the *Button Label* wont change the *Title* immediately. Restart Stream Deck.
