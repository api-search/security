---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paradoxinteractive.com
  spf: true
hosts:
- cert_expires: Mar 15 22:00:22 2027 GMT
  host: paradoxinteractive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Paradox Interactive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paradox Interactive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paradox Interactive
provider_slug: paradox-interactive
slug: paradox-interactive-domain-security
source_filename: paradox-interactive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paradoxinteractive.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 15 22:00:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paradoxinteractive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradox-interactive/refs/heads/main/security/paradox-interactive-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- VideoGames
- GrandStrategy
- Simulation
- Community
---
