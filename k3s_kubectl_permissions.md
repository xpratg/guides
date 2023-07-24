<h1>Resolve k3s kubectl permission problems</h1>
<h3>On server side execute commands:</h3>
<ol>
    <li>sudo vi /etc/systemd/system/k3s.service.env</li>
    <li>press insert/i, add K3S_KUBECONFIG_MODE="644" and press esc, type :wq and press enter</li>
    <li>sudo systemctl restart k3s</li>
</ol>

<h4>Source:</h4>
https://0to1.nl/post/k3s-kubectl-permission/