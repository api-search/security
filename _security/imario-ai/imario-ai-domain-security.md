---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imario.ai
  spf: true
hosts:
- cert_expires: Feb  6 20:12:05 2027 GMT
  host: imario.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: iMario Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iMario, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: iMario
provider_slug: imario-ai
slug: imario-ai-domain-security
source_filename: imario-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imario.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 20:12:05 2027 GMT\n  hsts: false\ndomains:\n- domain: imario.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/imario-ai/security/imario-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- SyntheticAudiences
- Marketing
- Data
---
