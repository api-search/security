---
api_specs:
- filename: ansible-auth-api-openapi.yml
  format: yaml
  label: Ansible Auth API
  slug: ansible-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-auth-api-openapi.yml
- filename: ansible-credentials-api-openapi.yml
  format: yaml
  label: Ansible Credentials API
  slug: ansible-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-credentials-api-openapi.yml
- filename: ansible-hosts-api-openapi.yml
  format: yaml
  label: Ansible Hosts API
  slug: ansible-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-hosts-api-openapi.yml
- filename: ansible-inventories-api-openapi.yml
  format: yaml
  label: Ansible Inventories API
  slug: ansible-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-inventories-api-openapi.yml
- filename: ansible-job-templates-api-openapi.yml
  format: yaml
  label: Ansible Job Templates API
  slug: ansible-job-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-job-templates-api-openapi.yml
- filename: ansible-jobs-api-openapi.yml
  format: yaml
  label: Ansible Jobs API
  slug: ansible-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-jobs-api-openapi.yml
- filename: ansible-organizations-api-openapi.yml
  format: yaml
  label: Ansible Organizations API
  slug: ansible-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-organizations-api-openapi.yml
- filename: ansible-projects-api-openapi.yml
  format: yaml
  label: Ansible Projects API
  slug: ansible-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-projects-api-openapi.yml
- filename: ansible-schedules-api-openapi.yml
  format: yaml
  label: Ansible Schedules API
  slug: ansible-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-schedules-api-openapi.yml
- filename: ansible-users-api-openapi.yml
  format: yaml
  label: Ansible Users API
  slug: ansible-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-users-api-openapi.yml
- filename: ansible-workflow-job-templates-api-openapi.yml
  format: yaml
  label: Ansible Workflow Job Templates API
  slug: ansible-workflow-job-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-workflow-job-templates-api-openapi.yml
- filename: ansible-workflow-jobs-api-openapi.yml
  format: yaml
  label: Ansible Workflow Jobs API
  slug: ansible-workflow-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/openapi/ansible-workflow-jobs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ansible.com
  spf: true
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: www.ansible.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:36:59 2026 GMT
  host: docs.ansible.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 12:14:32 2026 GMT
  host: galaxy.ansible.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ansible Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ansible, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ansible
provider_slug: ansible
slug: ansible-domain-security
source_filename: ansible-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ansible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ansible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:36:59 2026 GMT\n  hsts: false\n- host: galaxy.ansible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 12:14:32 2026 GMT\n  hsts: false\ndomains:\n- domain: ansible.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansible/refs/heads/main/security/ansible-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Ansible
- Automation
- Configuration Management
- DevOps
- Infrastructure as Code
- Open-Source
- Orchestration
- Red Hat
---
