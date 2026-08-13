---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gosecure.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gosecure.net
  spf: true
hosts:
- cert_expires: Oct  5 04:17:13 2026 GMT
  host: www.gosecure.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 00:25:34 2026 GMT
  host: api.gosecure.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Countertack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CounterTack, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CounterTack
provider_slug: countertack
slug: countertack-domain-security
source_filename: countertack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gosecure.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:17:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gosecure.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 00:25:34 2026 GMT\n  hsts: null\ndomains:\n- domain: gosecure.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gosecure.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/countertack/refs/heads/main/security/countertack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Cybersecurity
- Endpoint Security
- Endpoint Detection and Response
- Managed Detection and Response
- Threat Detection
- Incident Response
- SIEM
---
