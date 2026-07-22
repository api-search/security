---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: om1.com
  spf: true
hosts:
- cert_expires: Oct  8 18:18:47 2026 GMT
  host: om1.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Om1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Om1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Om1
provider_slug: om1
slug: om1-domain-security
source_filename: om1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: om1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: om1.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/om1/refs/heads/main/security/om1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Real-World Data
- Real-World Evidence
- Artificial Intelligence
- Machine Learning
- Analytics
- Life Sciences
- Clinical Data
- Data
---
