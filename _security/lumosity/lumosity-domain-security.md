---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lumosity.com
  spf: true
hosts:
- cert_expires: Jan 10 00:00:18 2027 GMT
  host: lumosity.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lumosity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumosity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lumosity
provider_slug: lumosity
slug: lumosity-domain-security
source_filename: lumosity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumosity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 00:00:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: lumosity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumosity/refs/heads/main/security/lumosity-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Brain Training
- Cognitive Training
- Consumer Apps
- Health and Wellness
- Mobile
- Games
---
