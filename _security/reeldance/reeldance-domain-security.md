---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reeldance.ai
  spf: true
hosts:
- cert_expires: Feb  3 12:27:49 2027 GMT
  host: reeldance.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ReelDance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReelDance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ReelDance
provider_slug: reeldance
slug: reeldance-domain-security
source_filename: reeldance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reeldance.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 12:27:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reeldance.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/reeldance/security/reeldance-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Creative
- Video
- Image-to-Video
- Freemium
---
