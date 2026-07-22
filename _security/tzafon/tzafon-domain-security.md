---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lightcone.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tzafon.ai
  spf: true
hosts:
- cert_expires: Oct  4 09:39:29 2026 GMT
  host: docs.lightcone.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 03:05:29 2026 GMT
  host: api.tzafon.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tzafon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tzafon, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tzafon
provider_slug: tzafon
slug: tzafon-domain-security
source_filename: tzafon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.lightcone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:39:29 2026 GMT\n  hsts: false\n- host: api.tzafon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:05:29 2026 GMT\n  hsts: null\ndomains:\n- domain: lightcone.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tzafon.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tzafon/refs/heads/main/security/tzafon-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Computer Use Agents
- Browser Automation
- AI Agents
- Vision Language Models
- Cloud Computers
- Automation
---
