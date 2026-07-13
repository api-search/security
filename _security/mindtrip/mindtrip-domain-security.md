---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mindtrip.ai
  spf: true
hosts:
- cert_expires: Sep 14 16:55:47 2026 GMT
  host: mindtrip.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mindtrip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mindtrip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mindtrip
provider_slug: mindtrip
slug: mindtrip-domain-security
source_filename: mindtrip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindtrip.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:55:47 2026 GMT\n  hsts: false\ndomains:\n- domain: mindtrip.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindtrip/refs/heads/main/security/mindtrip-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Travel
- AI
- Agentic AI
- Itinerary Planning
- Booking
- Consumer
---
