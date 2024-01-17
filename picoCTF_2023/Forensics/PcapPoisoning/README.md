<h1>PcapPoisoning</h1>

<h2>Description</h2>
<blockquote>
  How about some hide and seek heh?<br/>
  Download this <a href="https://github.com/KhanhCQ1511/picoCTF/blob/main/picoCTF_2023/Forensics/PcapPoisoning/trace.pcap">file</a> and find the flag.
</blockquote>

<h2>Solution</h2>
<p>Run command:</p>
<p><code>strings trace.pcap | grep -b pico</code></p>

<p><b>Other solution:</b></p>
<p>Open file <code>trace.pcap</code> in <code>WhiteShark</code></p>
<p>Find <code>tcp.stream eq 1</code> on line filter. You can see the flag</p>

<p>Flag: <code>picoCTF{P64P_4N4L7S1S_SU55355FUL_fc4e803f}</code></p>
