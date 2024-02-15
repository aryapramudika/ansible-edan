# Ansible EDA(N) Example


## Installing EDA in Ubuntu 22

```
apt-get install openjdk-18 -y
pip install ansible-rulebook
ansible-galaxy collection install ansible.eda
```
## Run Rulebook

```
ansible-rulebook -i inventory -r rule.yml --verbose
```

## Testing using payload message "ms"

```
curl -H 'Content-Type: application/json' -d "{\"message\": \"ms\"}" 127.0.0.1:5000/endpoint
```
