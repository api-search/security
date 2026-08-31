---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fivelives.health
  spf: true
hosts:
- cert_expires: Sep  1 06:28:29 2026 GMT
  host: fivelives.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Five Lives Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Five Lives, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Five Lives
provider_slug: five-lives
slug: five-lives-domain-security
source_filename: five-lives-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fivelives.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 06:28:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fivelives.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/five-lives/refs/heads/main/security/five-lives-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Brain Health
- Dementia Prevention
- Cognitive Health
- Digital Health
- HealthTech
- Neuroscience
- Aging
- Mobile App
---
