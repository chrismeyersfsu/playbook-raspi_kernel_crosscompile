##playbook-raspi_kernel_crosscompile
Cross-compile the linux kernel, and modules, locally on your beefy machine. See http://mitchtech.net/raspberry-pi-kernel-compile/ for detailed instructions.

Edit `host_vars/localhost.yml` with your local machines password for sudo purposes.
```
ansible-playbook -i localhost.yml -vvv
```
When the playbook finishes you may copy `linux/kernel.img` `lib/modules/` and `lib/firmware/` to your raspberry pi