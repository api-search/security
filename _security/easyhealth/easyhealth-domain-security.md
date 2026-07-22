---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: easyhealth.com
  spf: true
hosts:
- cert_expires: Oct 15 21:15:46 2026 GMT
  host: www.easyhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Easyhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Easyhealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Easyhealth
provider_slug: easyhealth
slug: easyhealth-domain-security
source_filename: easyhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.easyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:15:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: easyhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easyhealth/refs/heads/main/security/easyhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medicare
- Value-Based Care
- Preventive Care
- Health Insurance
- Care Coordination
- In-Home Care
- Telehealth
- HEDIS
---
