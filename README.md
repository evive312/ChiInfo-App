<h1> Chicago Events Information App</h1>

### [YouTube Demonstration](https://youtube.com/shorts/Bk-qFDOZ-S8)

<h2>Description</h2>
Project consists of **two cooperative Android 15 (API 35) apps**:

* **Chooser App (App1)** – A simple launcher with two buttons. Each button shows a toast and broadcasts an implicit intent (`ACTION_SHOW_ATTRACTIONS` or `ACTION_SHOW_RESTAURANTS`).

* **Information App (App2)** – Receives those broadcasts via manifest-declared receivers and opens one of two activities:
  * **AttractionsActivity** – List of five Chicago attractions + WebView for the selected item.
  * **RestaurantsActivity** – List of five Chicago restaurants + WebView for the selected item.

Both activities start in single-pane mode (list only). After the user selects an item, the UI switches to a two-pane layout (list ≈ ⅓, WebView ≈ ⅔). State is retained with a shared `ViewModel`/`LiveData`.

<br />


<h2>Languages and Utilities Used</h2>

- <b>Java</b> (Activities, Fragments, BroadcastReceivers, ViewModel)
- <b>XML</b> (Layouts, Manifest, resources)
- <b>Android Jetpack</b> (ViewModel, LiveData, RecyclerView, WebView)

<h2>Environments Used </h2>

- <b>Android Studio Iguana</b>
- <b>Android 15 (API 35)</b> Pixel 8 emulator

<h2>Program walk-through:</h2>

<p align="center">
Chooser app with two buttons:<br/>
<img src="https://i.imgur.com/wodKef1.png" height="40%" width="40%" alt="Chooser App"/>
<br /><br />
Broadcast received – Information app opens RestaurantsActivity:<br/>
<img src="https://i.imgur.com/RspMu1P.jpeg" height="40%" width="40%" alt="Restaurants List"/>
<br /><br />
User taps “Portillo’s Hot Dogs” – two-pane layout appears:<br/>
<img src="https://i.imgur.com/a2Mzf8Z.png" height="40%" width="40%" alt="Two-Pane Layout"/>
<br /><br />
Options menu allows switching back to attractions:<br/>
<img src="https://i.imgur.com/8w9YWpK.png" height="40%" width="40%" alt="Options Menu"/>
<br /><br />
Attractions list after broadcast:<br/>
<img src="https://i.imgur.com/Va96jBA.png" height="40%" width="40%" alt="Attractions List"/>
</p>
