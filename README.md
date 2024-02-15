# Ansible EDA(N) Example

## Run Rulebook

```
ansible-rulebook -i inventory -r rule.yml --verbose
```

## Testing using payload message "ms"

```
curl -H 'Content-Type: application/json' -d "{\"message\": \"ms\"}" 127.0.0.1:5000/endpoint
```
