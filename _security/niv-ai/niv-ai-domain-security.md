---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: niv-ai.com
  spf: true
hosts:
- cert_expires: Dec  6 14:20:14 2026 GMT
  host: niv-ai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Niv Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Niv-AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Niv-AI
provider_slug: niv-ai
slug: niv-ai-domain-security
source_filename: niv-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: niv-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 14:20:14 2026 GMT\n  hsts: false\ndomains:\n- domain: niv-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/niv-ai/security/niv-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Artificial Intelligence
- Data Center
- Sustainability
---
