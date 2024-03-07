Create 2 instances.

One: Control.

Second: Target.

Create SSh connection b/w both through ssh-keygen.

Copy through cat /home/ubuntu/.ssh/id_rsa.pub in control instance.

Then paste in target instance through vi /home/ubuntu/.ssh/authorized_keys.

Create inventory file (vi) in control server.

[ec2_instance]
Private IP address ssh_ansible_user.

Create playbook.yml in control server.

Create wp-config.php.j2 file (vi) in control server.

**Do following tasks in target server**

**Find**

ls /etc/apache2/sites-available/.

**Create**

sudo vi /etc/apache2/sites-available/wordpress.conf

**Restart apache 2**

sudo a2ensite wordpress

sudo service apache2 restart
Create 
sudo vi /etc/apache2/sites-available/wordpress.conf
Restart apache 2
sudo a2ensite wordpress
sudo service apache2 restart
