---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pega.com
  spf: true
hosts:
- cert_expires: Apr 14 19:33:34 2027 GMT
  host: pega.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 14 19:33:34 2027 GMT
  host: docs.pega.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Pega Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pega, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pega
provider_slug: pega
slug: pega-domain-security
source_filename: pega-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pega.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 14 19:33:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pega.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 14 19:33:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pega.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pega/refs/heads/main/security/pega-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Low-Code
- Business Process Management
- Workflow-Automation
- CRM
- Decisioning
- Artificial Intelligence
- Enterprise
- Case Management
---
