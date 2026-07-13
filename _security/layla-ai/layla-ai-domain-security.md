---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: layla.ai
  spf: true
hosts:
- cert_expires: Sep 21 21:04:03 2026 GMT
  host: layla.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Layla Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Layla AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Layla AI
provider_slug: layla-ai
slug: layla-ai-domain-security
source_filename: layla-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: layla.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:04:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: layla.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layla-ai/refs/heads/main/security/layla-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Travel
- Itinerary Planning
- Conversational AI
- White Label
- Booking
- Consumer
---
