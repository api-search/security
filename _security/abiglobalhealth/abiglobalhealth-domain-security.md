---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abiglobalhealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abi.ai
  spf: true
hosts:
- cert_expires: Oct  8 14:48:53 2026 GMT
  host: www.abiglobalhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: docs.abi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: client-api.abi.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Abiglobalhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abi Global Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Abi Global Health
provider_slug: abiglobalhealth
slug: abiglobalhealth-domain-security
source_filename: abiglobalhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abiglobalhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 14:48:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.abi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\n- host: client-api.abi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: abiglobalhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: abi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abiglobalhealth/refs/heads/main/security/abiglobalhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Telehealth
- Virtual Care
- Digital Health
- Health Insurance
- Healthcare Navigation
- Artificial Intelligence
- Prescriptions
- Webhooks
- Ireland
---
