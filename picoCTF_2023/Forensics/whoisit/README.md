<h1>Who is it</h1>

<h2>Descreiption</h2>
<blockquote>
  Someone just sent you an email claiming to be Google's co-founder Larry Page but you suspect a scam.<br/>
  Can you help us identify whose mail server the email actually originated from?<br/>
  Download the email file <a href="https://github.com/KhanhCQ1511/picoCTF/blob/main/picoCTF_2023/Forensics/whoisit/email-export.eml">here</a>.<br/>
  Flag: picoCTF{FirstnameLastname}
</blockquote>

<h2>Solution</h2>
<p><code>cat email-export.eml</code></p>
<p>Find the line same the image below:</p>
<img src="https://github.com/KhanhCQ1511/picoCTF/blob/main/picoCTF_2023/Forensics/whoisit/whoisit(1).png"/>
<p>You can see the domain of designate ip is <code>173.249.33.206</code></p>
<p>Use <a href="https://www.whois.com/">whois.com</a> to find information about this id and you can see flag you want to find</p>
<p>Flag: <code>picoCTF{WilhelmZwalina}</code></p>
