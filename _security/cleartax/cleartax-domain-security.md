---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cleartax.in
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clear.in
  spf: true
hosts:
- cert_expires: Sep  1 13:18:13 2026 GMT
  host: docs.cleartax.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 14:51:52 2027 GMT
  host: api.clear.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cleartax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cleartax, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cleartax
provider_slug: cleartax
slug: cleartax-domain-security
source_filename: cleartax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.cleartax.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:18:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.clear.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 14:51:52 2027 GMT\n  hsts: null\ndomains:\n- domain: cleartax.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: clear.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleartax/refs/heads/main/security/cleartax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tax
- GST
- E-Invoicing
- Compliance
- Fintech
- Accounting
- India
- Financial Automation
- Government
---
