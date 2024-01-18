<h1>FindAndOpen</h1>

<h2>Description</h2>
<blockquote>
  Someone might have hidden the password in the trace file.<br/>
  Find the key to unlock this <a href="https://github.com/KhanhCQ1511/picoCTF/blob/main/picoCTF_2023/Forensics/FindAndOpen/dump.pcap">file</a>.<br/>
  <a  href="https://github.com/KhanhCQ1511/picoCTF/blob/main/picoCTF_2023/Forensics/FindAndOpen/flag.zip">This tracefile</a> might be good to analyze.<br/>
</blockquote>

<h2>Solution</h2>
<p><code>unzip flag.zip</code></p>
<p>After run this command, it ask you passsword to unzip and you don't know that</p>
<p>We still have one more unused file: <code>dump.pcap</code>.</p>
<p>Normally we will open that file with WhiteShark and search for information.</p>
<p>But I will use the command: <code>trings dump.pcap | grep password | grep flag</code></p>
<p>Lots of things appear. You can see a rather special sequence of characters is <code>iBwaWNvQ1RGe1</code></p>
<p>Next to that you will also see a note that this code has been split</p>
<p><code>strings dump.pcap| grep iBwaWNvQ1RGe1</code></p>
<p>You can see a special piece of code: <code>AABBHHPJGTFRLKVGhpcyBpcyB0aGUgc2VjcmV0OiBwaWNvQ1RGe1IzNERJTkdfTE9LZF8=</code></p>
<p>Decoding base64 the above code does nothing</p>
<p>Open WhiteShark and find above code, We discover a code hex in the above code: <code>VGhpcyBpcyB0aGUgc2VjcmV0OiBwaWNvQ1RGe1IzNERJTkdfTE9LZF8=</code></p>
<p>Decode base64 this code and result is <code>This is the secret: picoCTF{R34DING_LOKd_</code></p>
<p>Try it is password of file zip</p>
<p>Unzip and we get a file containing flag</p>
<p>Flag: <code>picoCTF{R34DING_LOKd_fil56_succ3ss_c2e6d949}</code></p>
