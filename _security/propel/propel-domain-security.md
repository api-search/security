---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: propel.app
  spf: true
hosts:
- cert_expires: Sep  5 04:13:52 2026 GMT
  host: www.propel.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Propel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Propel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Propel
provider_slug: propel
slug: propel-domain-security
source_filename: propel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.propel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 04:13:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: propel.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propel/refs/heads/main/security/propel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financial Services
- Government Benefits
- SNAP
- EBT
- Consumer Finance
- Mobile App
- Financial Health
---
