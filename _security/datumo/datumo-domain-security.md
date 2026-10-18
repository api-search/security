---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datumo.com
  spf: true
hosts:
- cert_expires: Dec 24 21:10:57 2026 GMT
  host: datumo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datumo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datumo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Datumo
provider_slug: datumo
slug: datumo-domain-security
source_filename: datumo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datumo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 21:10:57 2026 GMT\n  hsts: false\ndomains:\n- domain: datumo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datumo/refs/heads/main/security/datumo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Evaluation
- LLM
- Platform
---
