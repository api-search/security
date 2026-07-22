---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: incite.dev
  spf: true
hosts:
- cert_expires: Sep 18 00:13:51 2026 GMT
  host: incite.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Incite Interactive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Incite Interactive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Incite Interactive
provider_slug: incite-interactive
slug: incite-interactive-domain-security
source_filename: incite-interactive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incite.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 00:13:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: incite.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incite-interactive/refs/heads/main/security/incite-interactive-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming
- Artificial Intelligence
- Generative AI
- Agents
- Entertainment
- Interactive Media
---
