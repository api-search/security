---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: believe.com
  spf: true
hosts:
- cert_expires: Nov 12 07:33:21 2026 GMT
  host: www.believe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Believe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Believe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Believe
provider_slug: believe
slug: believe-domain-security
source_filename: believe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.believe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 07:33:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: believe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/believe/refs/heads/main/security/believe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Artist Development
- Songwriters
- Record Labels
- Publishers
- Distribution
---
