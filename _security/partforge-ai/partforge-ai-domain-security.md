---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: partforge.ai
  spf: true
hosts:
- cert_expires: Feb  3 12:50:38 2027 GMT
  host: partforge.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PartForge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PartForge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PartForge
provider_slug: partforge-ai
slug: partforge-ai-domain-security
source_filename: partforge-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partforge.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 12:50:38 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: partforge.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/partforge-ai/security/partforge-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- CAD
- 3D Printing
- Parametric Design
- Community
---
