---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: besample.app
  spf: true
hosts:
- cert_expires: Dec 25 06:50:43 2026 GMT
  host: besample.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Besample Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Besample, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Besample
provider_slug: besample
slug: besample-domain-security
source_filename: besample-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: besample.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 06:50:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: besample.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/besample/refs/heads/main/security/besample-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Research
- Participants
- Behavioral Science
- Data Platform
---
