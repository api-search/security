---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grok.me
  spf: false
hosts:
- cert_expires: Nov 18 05:18:32 2026 GMT
  host: asgardian-village.grok.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grok Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asgardian Village · Canadian house, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Asgardian Village · Canadian house
provider_slug: grok-me
slug: grok-me-domain-security
source_filename: grok-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: 'The TLS/HSTS row is the tenant host asgardian-village.grok.me and is what a client of this provider sees. The\n  domains[] row is the registrable domain grok.me, which is xAI''s Cloudflare zone (Grok app hosting; grok.me 301s to\n  grok.com) — its DNSSEC/CAA/SPF/DMARC posture belongs to the platform operator (all/xai), not to Asgardian Village,\n  which controls no DNS of its own.'\nhosts:\n- host: asgardian-village.grok.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 05:18:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: grok.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grok-me/refs/heads/main/security/grok-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- A2A
- AI Agents
- Agent Discovery
- Community
- Maker
- Hydroponics
- 3D Printing
- Canada
- Grok App
---
