---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: entyrecare.com
  spf: true
hosts:
- cert_expires: Aug 29 13:44:04 2026 GMT
  host: entyrecare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Entyre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entyre Care, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Entyre Care
provider_slug: entyre
slug: entyre-domain-security
source_filename: entyre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: entyrecare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 13:44:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: entyrecare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entyre/refs/heads/main/security/entyre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Home Health Care
- Caregiving
- Family Caregiver
- Medicaid
- Health Services
- Elder Care
---
