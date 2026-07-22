---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: basepowercompany.com
  spf: true
hosts:
- cert_expires: Oct 14 11:17:18 2026 GMT
  host: www.basepowercompany.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Base Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Base Power, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Base Power
provider_slug: base-power
slug: base-power-domain-security
source_filename: base-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.basepowercompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 11:17:18 2026 GMT\n  hsts: false\ndomains:\n- domain: basepowercompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/base-power/refs/heads/main/security/base-power-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Clean Energy
- Energy
- Home Battery
- Energy Storage
- Electricity
- Grid
- Retail Electric Provider
- Texas
- Illinois
---
