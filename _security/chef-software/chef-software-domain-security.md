---
api_specs:
- filename: chef-software-applications-applications-openapi.json
  format: json
  label: Chef Automate API
  slug: chef-automate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef-software/refs/heads/main/openapi/chef-software-applications-applications-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chef.io
  spf: true
hosts:
- cert_expires: Aug 20 22:43:43 2026 GMT
  host: docs.chef.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 19:40:25 2026 GMT
  host: automate.chef.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chef Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chef Software, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chef Software
provider_slug: chef-software
slug: chef-software-domain-security
source_filename: chef-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.chef.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:43:43 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: automate.chef.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 19:40:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chef.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chef-software/refs/heads/main/security/chef-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DevOps
- Infrastructure Automation
- Configuration Management
- Compliance
- Security
- Infrastructure as Code
- Cloud
- Continuous Compliance
- Node Management
---
