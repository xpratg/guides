<h1>Avoid ssh connection to hang</h1>
<h3>On server side execute commands:</h3>
<ol>
    <li>sudo vi /etc/ssh/sshd_config</li>
    <li>Type /ClientAliveInterval and press enter</li>
    <li>Press insert/i key</li>
    <li>Remove # and change value to 60</li>
    <li>Press esc and type :wq</li>
    <li>service sshd restart</li>
</ol>

<h4>Source:</h4>
https://unix.stackexchange.com/questions/200239/how-can-i-keep-my-ssh-sessions-from-freezing