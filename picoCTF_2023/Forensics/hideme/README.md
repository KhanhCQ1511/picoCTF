<h1>hideme</h1>

<h2>Description</h2>
<blockquote>
  Every file gets a flag.<br/>
  The SOC analyst saw one image been sent back and forth between two people.<br/>
  They decided to investigate and found out that there was more than what meets the eye <a href="picoCTF_2023/Forensics/hideme/flag.png">here</a>.
</blockquote>

<h2>Solution</h2>
<blockquote>Note: Use binwalk to solve this prolem</blockquote>
<p><code>binwalk flag.png</code></p>
<p>After run this <code>command</code> picture file become <code>zip</code> with extention <code>.png</code></p>
<p>Unzip file: <code>unzip flag.png</code></p>
<p>After unzipping the file, <code>secret folder</code> will appear</p>
<p><code>ls</code></p>
<p><code>cd secret</code></p>
<p>open file <code>flag.png</code> in folder <code>secret</code> will reviceve flag</p>
<p></p>
<p>Flag: <code>picoCTF{Hiddinng_An_imag3_within_@n_ima93_ad9f6587}</code></p>
