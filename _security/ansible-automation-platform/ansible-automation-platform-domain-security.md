---
api_specs:
- filename: ansible-controller-api.yaml
  format: yaml
  label: Ansible Automation Controller API
  slug: controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansible-automation-platform/refs/heads/main/openapi/ansible-controller-api.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ansible.com
  spf: true
hosts:
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
name: Ansible Automation Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ansible Automation Platform, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ansible Automation Platform
provider_slug: ansible-automation-platform
slug: ansible-automation-platform-domain-security
source_filename: ansible-automation-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.ansible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:36:59 2026 GMT\n  hsts: false\n- host: galaxy.ansible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 12:14:32 2026 GMT\n  hsts: false\ndomains:\n- domain: ansible.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansible-automation-platform/refs/heads/main/security/ansible-automation-platform-domain-security.yml
summary_line: TLSv1.3
tags:
- Automation
- Configuration Management
- DevOps
- Infrastructure as Code
- Orchestration
---
