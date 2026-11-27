---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moonscroll.ai
  spf: false
hosts:
- cert_expires: Jan 13 04:46:58 2027 GMT
  host: moonscroll.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MoonScroll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoonScroll, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: MoonScroll
provider_slug: moonscroll-ai
slug: moonscroll-ai-domain-security
source_filename: moonscroll-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moonscroll.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 04:46:58 2027 GMT\n  hsts: false\ndomains:\n- domain: moonscroll.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/moonscroll-ai/security/moonscroll-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Artificial Intelligence
- Analytics
- Short-form
- Marketing
---
