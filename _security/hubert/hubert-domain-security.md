---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hubert.ai
  spf: true
hosts:
- cert_expires: Jan  7 16:30:19 2027 GMT
  host: hubert.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hubert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hubert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hubert
provider_slug: hubert
slug: hubert-domain-security
source_filename: hubert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hubert.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 16:30:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hubert.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubert/refs/heads/main/security/hubert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Hiring
- Recruiting
- Automation
- Software-as-a-Service
---
