---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: altara.co
  spf: true
hosts:
- cert_expires: Sep 13 23:32:31 2026 GMT
  host: www.altara.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Altara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Altara, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Altara
provider_slug: altara
slug: altara-domain-security
source_filename: altara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.altara.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:32:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: altara.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altara/refs/heads/main/security/altara-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Deep Tech
- Artificial Intelligence
- AI Agents
- Physical Sciences
- Semiconductors
- Materials Science
- Manufacturing
- Scientific Data
- Failure Analysis
---
