---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: centrl.ai
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: centrl.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Centrly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centrly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Centrly
provider_slug: centrly
slug: centrly-domain-security
source_filename: centrly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centrl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: centrl.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrly/refs/heads/main/security/centrly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Integration
- Workflow Automation
- Software-as-a-Service
- Enterprise
---
