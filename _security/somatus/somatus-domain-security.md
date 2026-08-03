---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: somatus.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: renaliq.com
  spf: false
hosts:
- cert_expires: Sep 13 22:52:19 2026 GMT
  host: somatus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 18:13:30 2027 GMT
  host: connect.renaliq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Somatus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Somatus, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Somatus
provider_slug: somatus
slug: somatus-domain-security
source_filename: somatus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: somatus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:52:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.renaliq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 18:13:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: somatus.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: renaliq.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/somatus/refs/heads/main/security/somatus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Kidney Care
- Value-Based Care
- Chronic Care Management
- Population Health
- Health Plans
- Nephrology
- Care Management
- Predictive Analytics
---
