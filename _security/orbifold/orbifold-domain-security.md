---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: orbifold.ai
  spf: true
hosts:
- cert_expires: Jan  1 07:15:56 2027 GMT
  host: orbifold.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orbifold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbifold, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Orbifold
provider_slug: orbifold
slug: orbifold-domain-security
source_filename: orbifold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbifold.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 07:15:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orbifold.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/orbifold/security/orbifold-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Data
- Infrastructure
- Multimodal
---
