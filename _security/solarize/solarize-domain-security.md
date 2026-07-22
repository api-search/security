---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: solarize.de
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: solarize.energy
  spf: false
hosts:
- cert_expires: Sep 24 15:46:46 2026 GMT
  host: www.solarize.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 05:19:30 2026 GMT
  host: api-docs.solarize.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 05:19:30 2026 GMT
  host: api.solarize.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solarize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solarize, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Solarize
provider_slug: solarize
slug: solarize-domain-security
source_filename: solarize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solarize.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:46:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.solarize.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 05:19:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.solarize.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 05:19:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: solarize.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: solarize.energy\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solarize/refs/heads/main/security/solarize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Billing
- Metering
- Utilities
- Meter-to-Cash
- SaaS
---
