<h1 align="center">
  <pre style="line-height:0.9; margin:0; font-family:monospace;">
  ____  _       _    ____  _   _  __      __  _  __
 / ___|| | __ _| |_ / ___|| | | | \ \    / / | |/ _|
 \___ \| |/ _` | __| |    | |_| |  \ \/\/ /  | | |_
  ___) | | (_| | |_| |___ |  _  |   \_/\_/   | |  _|
 |____/|_|\__,_|\__|\____||_| |_|            |_|
  </pre>
</h1>

<div style="text-align:center; padding: 16px;">
  <div class="typewriter">
    <h2>/* booting... */</h2>
    <p id="typer"></p>
  </div>
</div>

<style>
/* Typewriter core — GitHub may allow this, but if not use plain text below */
.typewriter { font-family: "Courier New", monospace; color: #9be9a8; background: #0b0f12; padding: 16px; border-radius: 8px; display: inline-block; }
#typer { white-space: pre; font-size: 16px; }
.cursor { display:inline-block; width:10px; background:#9be9a8; margin-left:3px; animation: blink 1s steps(2) infinite; vertical-align: middle; }
@keyframes blink { 50% { opacity: 0 } }
</style>

<script>
/* Pure JS typewriter — GitHub README will not execute scripts. This is for demo/hosting pages.
   For GitHub profile READMEs the visual may be limited but the text below remains great.
*/
const lines = [
  "root@matrix:~$ echo 'hello. i'm Ibrahim — cyber curious, packet whisperer, and coffee-powered dev.'",
  "root@matrix:~$ cat skills.txt",
  " - Networking: CCNA-style routing & switching (lab-hardened)",
  " - Linux: shell scripting, servers, and config-fu",
  " - Security: ethical hacking fundamentals, IDS/IPS tinkering",
  " - Tools: Docker, Nginx, Apache, Ollama experiments",
  "root@matrix:~$ echo 'always learning. always curious.'"
];

let i = 0, j = 0, out = "";
const el = { typer: document.getElementById("typer") };
function step() {
  if (i >= lines.length) {
    el.typer.innerHTML = out + "<span class='cursor'>&nbsp;</span>";
    return;
  }
  const line = lines[i];
  if (j < line.length) {
    out += line[j++];
    el.typer.textContent = out;
    setTimeout(step, 28 + Math.random()*40);
  } else {
    out += "\n";
    i++; j = 0;
    setTimeout(step, 400);
  }
}
step();
</script>

<!-- Plain fallback content so your README still looks great even without scripts/styles -->
<details>
<summary>Text fallback (if animations are disabled)</summary>

