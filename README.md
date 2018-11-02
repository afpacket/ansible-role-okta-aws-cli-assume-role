# ansible-role-okta-aws-cli-assume-role
Ansible role to automate the installation of [okta-aws-cli-assume-role](https://github.com/oktadeveloper/okta-aws-cli-assume-role)

## Sample Playbook
In this example, the variable values are the same as in defaults. Set these values appropriately based on your organization.
```
- hosts: localhost
  connection: local
  vars:
    OKTA_ORG: "acmecorp.okta.com.changeme.local"
    OKTA_AWS_APP_URL: "https://acmecorp.oktapreview.com.changeme.local/home/amazon_aws/0oa5zrwfs815KJmVF0h7/137"
    OKTA_USERNAME: "USERNAME"
    OKTA_BROWSER_AUTH: "false"
  roles:
    - ansible-role-okta-aws-cli-assume-role  
```
