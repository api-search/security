---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: archimetis.ai
  spf: true
hosts:
- cert_expires: Sep 26 18:47:24 2026 GMT
  host: www.archimetis.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Archimetis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archimetis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Archimetis
provider_slug: archimetis
slug: archimetis-domain-security
source_filename: archimetis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.archimetis.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:47:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: archimetis.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archimetis/refs/heads/main/security/archimetis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Industrial
- Refining
- Chemicals
- Process Industries
- Operational Intelligence
- Energy
- Manufacturing
---
