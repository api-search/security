---
api_specs:
- filename: documentation
  format: yaml
  label: ProcessMaker Platform RESTful API
  slug: processmaker-platform-api
  spec_type: OpenAPI
  url: https://{organization}.processmaker.net/api/documentation
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: processmaker.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Sep  6 23:14:38 2026 GMT
  host: www.processmaker.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 17:00:10 2026 GMT
  host: processmaker.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Processmaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProcessMaker, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ProcessMaker
provider_slug: processmaker
slug: processmaker-domain-security
source_filename: processmaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.processmaker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:14:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: processmaker.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: processmaker.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/security/processmaker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BPM
- Business Process Management
- Workflow Automation
- BPMN 2.0
- Low-Code
- Intelligent Automation
- Process Design
- Case Management
- Task Management
- Enterprise Integration
---
