
## Getting Started

Follow these steps to set up and deploy the application:

### 1. Vault Password

Add your vault password to `vault/pass.txt`.

### 2. Add Database Secrets

Add your database credentials to the `vault/secrets.yaml` and run `ansible-vault encrypt secrets.yaml --vault-password-file pass.txt` command.

```yaml
db_name: your_database_name
db_user: your_database_user
db_password: your_database_password
db_host: your_database_host
db_port: your_database_port
```

### 3. Add Your Hosts

Add your hosts to the `inventory/hosts.ini` file.

### 4. Access the application

Open web browser and access the application at application_host_ip:5000

### 4. Run The Playbook

In the root folder run `ansible-playbook ./playbooks/playbook.yaml` command to run the ansible scripts.
