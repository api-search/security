---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: preemadonna.com
  spf: true
hosts:
- cert_expires: Sep 13 06:16:20 2026 GMT
  host: preemadonna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Preemadonna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Preemadonna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Preemadonna
provider_slug: preemadonna
slug: preemadonna-domain-security
source_filename: preemadonna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: preemadonna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 06:16:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: preemadonna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preemadonna/refs/heads/main/security/preemadonna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Consumer Electronics
- Hardware
- Nail Art
- Beauty
- AI
- Mobile App
- Creator Marketplace
---
