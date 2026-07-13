---
api_specs:
- filename: commvault-rest-openapi.yml
  format: yaml
  label: Commvault REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commvault/refs/heads/main/openapi/commvault-rest-openapi.yml
- filename: commvault-command-center-openapi.yml
  format: yaml
  label: Commvault Command Center API
  slug: command-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commvault/refs/heads/main/openapi/commvault-command-center-openapi.yml
- filename: commvault-automation-openapi.yml
  format: yaml
  label: Commvault Automation API
  slug: automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commvault/refs/heads/main/openapi/commvault-automation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commvault.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: cloud.commvault.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: documentation.commvault.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: webserver.commvault.com
  https: false
kind: domain-security
layout: security
method: probed
name: Commvault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commvault, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Commvault
provider_slug: commvault
slug: commvault-domain-security
source_filename: commvault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.commvault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\n- host: documentation.commvault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webserver.commvault.com\n  https: false\ndomains:\n- domain: commvault.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commvault/refs/heads/main/security/commvault-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backup
- Cloud Storage
- Cyber Recovery
- Data Management
- Data Protection
- Disaster Recovery
- Enterprise Software
---
