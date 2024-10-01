# Commands

Below are the commands that you can easily copy by tapping the button.

### Command 1
```bash
<pre><code id="pkg install python">npm install package-name</code></pre>
<button onclick="copyToClipboard('pkg install python')">Tap to Copy</button>

### Command 2
```bash
<pre><code id="command2">git clone https://github.com/APKSHADOWESP/SEEDS</code></pre>
<button onclick="copyToClipboard('command2')">Tap to Copy</button>

<script>
function copyToClipboard(commandId) {
    var copyText = document.getElementById(commandId);
    var textArea = document.createElement("textarea");
    textArea.value = copyText.textContent || copyText.innerText;
    document.body.appendChild(textArea);
    textArea.select();
    document.execCommand("copy");
    document.body.removeChild(textArea);
    alert("Command copied: " + textArea.value);
}
</script>
