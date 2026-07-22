---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: knotch.it
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: knotch.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knotch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knotch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Knotch
provider_slug: knotch
slug: knotch-domain-security
source_filename: knotch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knotch.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: knotch.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knotch/refs/heads/main/security/knotch-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Content Intelligence
- Content Marketing
- Analytics
- Artificial Intelligence
- Personalization
- Marketing Technology
- Agentic Web
---
