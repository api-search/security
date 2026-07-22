---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cooklist.com
  spf: true
hosts:
- cert_expires: Sep 25 09:28:45 2026 GMT
  host: cooklist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cooklist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cooklist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cooklist
provider_slug: cooklist
slug: cooklist-domain-security
source_filename: cooklist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cooklist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 09:28:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cooklist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooklist/refs/heads/main/security/cooklist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agentic Commerce
- Grocery
- Retail
- AI Assistant
- Model Context Protocol
- Recipes
- Meal Planning
- E-Commerce
- Personalization
---
