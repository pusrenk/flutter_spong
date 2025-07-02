<h1 class="code-line" data-line-start=0 data-line-end=1 ><a id="spongflutter_0"></a>spong-flutter</h1>
<p class="has-line-data" data-line-start="1" data-line-end="2">spong flutter for mobile</p>
<p class="has-line-data" data-line-start="4" data-line-end="5">Follow the official documentation of Flutter to set up: <a href="https://docs.flutter.dev/get-started/install/windows/mobile">https://docs.flutter.dev/get-started/install/windows/mobile</a></p>
<p class="has-line-data" data-line-start="6" data-line-end="7">NOTE*: u don’t need to setup android studio if u not running the apps in there, u only need the android SDK 35 and good to go.</p>
<p class="has-line-data" data-line-start="9" data-line-end="10">----Common Commands----</p>
<p class="has-line-data" data-line-start="11" data-line-end="12">–Flutter–</p>
<ul>
<li class="has-line-data" data-line-start="12" data-line-end="13">flutter clean          : Clean build files</li>
<li class="has-line-data" data-line-start="13" data-line-end="14">flutter pub get        : Fetch dependencies</li>
<li class="has-line-data" data-line-start="14" data-line-end="15">flutter doctor         : Diagnose setup issues</li>
<li class="has-line-data" data-line-start="15" data-line-end="16">flutter devices        : List connected devices</li>
<li class="has-line-data" data-line-start="16" data-line-end="17">flutter build apk      : Build release APK</li>
<li class="has-line-data" data-line-start="17" data-line-end="18">flutter run            : run the project</li>
<li class="has-line-data" data-line-start="18" data-line-end="20">flutter --version      : version check</li>
</ul>
<p class="has-line-data" data-line-start="20" data-line-end="21">–ADB–</p>
<ul>
<li class="has-line-data" data-line-start="21" data-line-end="22">adb devices                     : list connected devices</li>
<li class="has-line-data" data-line-start="22" data-line-end="23">adb connect &lt;ip&gt;:&lt;port&gt;         : connect devices</li>
<li class="has-line-data" data-line-start="23" data-line-end="24">adb pair &lt;ip&gt;:&lt;port&gt;            : pair devices over wifi</li>
<li class="has-line-data" data-line-start="24" data-line-end="25">adb disconnect                  : disconnect all devices</li>
<li class="has-line-data" data-line-start="25" data-line-end="26">adb tcpip 5555                  : make static port</li>
<li class="has-line-data" data-line-start="26" data-line-end="27">adb kill-server                 : stop the adb server</li>
<li class="has-line-data" data-line-start="27" data-line-end="28">adb start-server                : start the adb server</li>
<li class="has-line-data" data-line-start="28" data-line-end="29">adb logcat                      : print log</li>
</ul>
<h2 class="code-line" data-line-start=31 data-line-end=32 ><a id="_Development_Environment_31"></a>🧩 Development Environment</h2>
<table class="table table-striped table-bordered">
<thead>
<tr>
<th>Tool</th>
<th>Version</th>
</tr>
</thead>
<tbody>
<tr>
<td>Flutter</td>
<td>3.32.4</td>
</tr>
<tr>
<td>Dart</td>
<td>3.8.1</td>
</tr>
<tr>
<td>Android SDK</td>
<td>35</td>
</tr>
<tr>
<td>Android Build Tools</td>
<td>35.0.0</td>
</tr>
<tr>
<td>Java (JDK)</td>
<td>17.0.9 (LTS)</td>
</tr>
<tr>
<td>Gradle</td>
<td>8.3</td>
</tr>
</tbody>
</table>
<p class="has-line-data" data-line-start="42" data-line-end="43">NOTE*: for gradle ver i still don’t know the compatibilty across flutter, dart, java, but personally i use 8.3</p>
<p class="has-line-data" data-line-start="45" data-line-end="46">----How to run the apps on real devices(Android)----</p>
<p class="has-line-data" data-line-start="47" data-line-end="48">There is some way to run it on your phone</p>
<ol>
<li class="has-line-data" data-line-start="48" data-line-end="49">Using your hotspot phone</li>
<li class="has-line-data" data-line-start="49" data-line-end="50">Connect it with USB cable(USB debug)</li>
<li class="has-line-data" data-line-start="50" data-line-end="52">Connect it wireless using the same wifi router</li>
</ol>
<p class="has-line-data" data-line-start="52" data-line-end="53">i recommend to use wireless method since that is the most convenient way</p>
<p class="has-line-data" data-line-start="54" data-line-end="55">NOTE* All of this way is need to use ADB(Android Debug Bridge), adb comes in with the android SDK(assuming you’re already download Android SDK 35)</p>
<p class="has-line-data" data-line-start="57" data-line-end="58">----How to connect it wireless----</p>
<ol>
<li class="has-line-data" data-line-start="59" data-line-end="69">
<p class="has-line-data" data-line-start="59" data-line-end="60">Go to Developer Options</p>
<ul>
<li class="has-line-data" data-line-start="61" data-line-end="63">
<p class="has-line-data" data-line-start="61" data-line-end="62">Open your phone’s Settings</p>
</li>
<li class="has-line-data" data-line-start="63" data-line-end="65">
<p class="has-line-data" data-line-start="63" data-line-end="64">Scroll to “About phone”</p>
</li>
<li class="has-line-data" data-line-start="65" data-line-end="67">
<p class="has-line-data" data-line-start="65" data-line-end="66">Tap “Build number” 7 times until it says “You are now a developer”</p>
</li>
<li class="has-line-data" data-line-start="67" data-line-end="69">
<p class="has-line-data" data-line-start="67" data-line-end="68">Go back to Settings &gt; System &gt; Developer Options (or just search for “Developer options”)</p>
</li>
</ul>
</li>
<li class="has-line-data" data-line-start="69" data-line-end="81">
<p class="has-line-data" data-line-start="69" data-line-end="70">Enable USB Debugging</p>
<ul>
<li class="has-line-data" data-line-start="71" data-line-end="73">
<p class="has-line-data" data-line-start="71" data-line-end="72">In Developer Options, find and enable USB debugging</p>
</li>
<li class="has-line-data" data-line-start="73" data-line-end="75">
<p class="has-line-data" data-line-start="73" data-line-end="74">connect your phone to your pc via USB cable</p>
</li>
<li class="has-line-data" data-line-start="75" data-line-end="77">
<p class="has-line-data" data-line-start="75" data-line-end="76">run ‘adb devices’ to verify your devices is detected</p>
</li>
<li class="has-line-data" data-line-start="77" data-line-end="79">
<p class="has-line-data" data-line-start="77" data-line-end="78">run ‘adb tcpip 5555’ to make ip static</p>
</li>
<li class="has-line-data" data-line-start="79" data-line-end="81">
<p class="has-line-data" data-line-start="79" data-line-end="80">wait for a while and disconnect your phone</p>
</li>
</ul>
</li>
<li class="has-line-data" data-line-start="81" data-line-end="85">
<p class="has-line-data" data-line-start="81" data-line-end="82">Enable Wireless Debugging</p>
<ul>
<li class="has-line-data" data-line-start="83" data-line-end="85">In Developer Options, find and enable Wireless debugging</li>
</ul>
</li>
<li class="has-line-data" data-line-start="85" data-line-end="92">
<p class="has-line-data" data-line-start="85" data-line-end="86">Tap on “Wireless debugging”</p>
<ul>
<li class="has-line-data" data-line-start="87" data-line-end="89">
<p class="has-line-data" data-line-start="87" data-line-end="88">This opens the wireless debugging options</p>
</li>
<li class="has-line-data" data-line-start="89" data-line-end="91">
<p class="has-line-data" data-line-start="89" data-line-end="90">You can see your phone IP &amp; Port there, but since we already make static Port which is easier to connect, we can ignore the phone Port</p>
</li>
<li class="has-line-data" data-line-start="91" data-line-end="92">
<p class="has-line-data" data-line-start="91" data-line-end="92">On your run ‘adb connect &lt;ip&gt;:&lt;port&gt;’</p>
</li>
</ul>
</li>
</ol>