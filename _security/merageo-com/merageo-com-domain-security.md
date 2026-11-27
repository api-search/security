---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: merageo.com
  spf: true
hosts:
- cert_expires: Jan 16 22:58:30 2027 GMT
  host: merageo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: meraGEO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for meraGEO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: meraGEO
provider_slug: merageo-com
slug: merageo-com-domain-security
source_filename: merageo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merageo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 22:58:30 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: merageo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/merageo-com/security/merageo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Branding
- Analytics
- Monitoring
- Software-as-a-Service
---
