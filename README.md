# coherence-playbook
Mac workstation playbook


```bash
xcode-select --install
sudo easy_install pip
sudo pip install ansible
mkdir workspaces && cd workspaces
git clone git@github.com:kwoods/coherence-playbook.git
cd mac-dev-playbook
ansible-galaxy install -r requirements.yml

ansible-playbook -i inventory --become main.yml

cd ~/dotfiles
bin/install
bin/setup_osx
```
