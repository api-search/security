---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: learnatnoon.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: learnatnoon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noon Academy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noon Academy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Noon Academy
provider_slug: noon-academy
slug: noon-academy-domain-security
source_filename: noon-academy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learnatnoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: learnatnoon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noon-academy/refs/heads/main/security/noon-academy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- EdTech
- Social Learning
- Online Learning
- Tutoring
---
