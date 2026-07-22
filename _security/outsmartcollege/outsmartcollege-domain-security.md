---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: Quarntine
  dnssec: false
  domain: outsmartcollege.com
  spf: true
hosts:
- cert_expires: Sep  3 04:38:27 2026 GMT
  host: outsmartcollege.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outsmartcollege Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outsmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=Quarntine).'
provider_name: Outsmart
provider_slug: outsmartcollege
slug: outsmartcollege-domain-security
source_filename: outsmartcollege-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outsmartcollege.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 04:38:27 2026 GMT\n  hsts: false\ndomains:\n- domain: outsmartcollege.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: Quarntine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outsmartcollege/refs/heads/main/security/outsmartcollege-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- EdTech
- Artificial Intelligence
- Learning
- Higher Education
- Mobile
- Consumer
---
