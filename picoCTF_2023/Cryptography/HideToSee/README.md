<h1>HideToSee</h1>

<h2>Description</h2>
<blockquote>
  How about some hide and seek heh? Look at this image <a href="https://github.com/KhanhCQ1511/picoCTF/blob/main/picoCTF_2023/Cryptography/HideToSee/atbash.jpg">here</a>.
</blockquote>

<h2>Solution</h2>
<p><strong>Hint: </strong>Download the image and try to extract it.</p>
<p><code>steghide extract -sf atbash.jpg</code>(no enter passphrase)</p>
<p>After run this command file <code>.jpg</code> extract to file <code>encrypted.txt</code></p>
<p><code>cat encrypted.txt</code> and we can see special code: <code>krxlXGU{zgyzhs_xizxp_05y2z65z}</code></p>
<p>Use <a hred="https://www.dcode.fr/atbash-cipher">atbash cipher</a> to decode this code and we receive flag</p>
<p>Flag: <code>picoCTF{atbash_crack_05b2a65a}</code></p>
