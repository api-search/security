---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: q.bio
  spf: true
hosts:
- cert_expires: Aug 25 00:06:31 2026 GMT
  host: q.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Q Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Q Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Q Bio
provider_slug: q-bio
slug: q-bio-domain-security
source_filename: q-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: q.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:06:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: q.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/q-bio/refs/heads/main/security/q-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Preventive Health
- Medical Imaging
- MRI
- Genomics
- Longevity
- Health Data
---
