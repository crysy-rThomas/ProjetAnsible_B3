<h1>ProjectAnsible_B3</h1>

<p>This project uses Ansible to automate the installation and configuration of the <code>zzet.rbenv</code> role on a target machine. To use this project, you need to follow the steps outlined below:</p>

<h2>Prerequisites</h2>

<p>Before running the Ansible playbook, you need to ensure that Ansible is installed on your machine. You can install Ansible by following the instructions on the <a href="https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html" target="_new">official Ansible website</a>.</p>

<p>Additionally, you will need to install the <code>zzet.rbenv</code> role. You can do this by running the following command:</p>

<pre><code>ansible-galaxy install zzet.rbenv
</code></pre>

<h2>Configuration</h2>

<h3>Hosts</h3>

<p>You need to specify the host or hosts that you want to target in the <code>hosts.ini</code> file. This file should contain the IP address or domain name of each host that you want to target, separated by commas. For example:</p>

<pre>
<span>[webservers]</span>
<span>192.168.1.101</span>
</code></pre>

<h3>Variables</h3>

<p>To configure the playbook, you will need to modify the variables in the <code>group_vars/all</code> file. This file contains the default variables that will be used when running the playbook. You should modify these variables according to your needs.</p>

<h2>Running the Playbook</h2>

<p>To run the playbook, execute the following command:</p>

<pre><code>ansible-playbook -i hosts.ini playbooks/main-playbook.yml</code></pre>

<p>This will execute the main playbook, which will install and configure <code>zzet.rbenv</code> on the target machine.</p>

<h2>Contributing</h2>

<p>If you would like to contribute to this project, please feel free to submit a pull request. We welcome contributions of all kinds, including bug fixes, feature requests, and documentation improvements.</p>
