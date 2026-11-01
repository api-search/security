---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: relume.ai
  spf: true
hosts:
- cert_expires: Jan 24 08:04:32 2027 GMT
  host: relume.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Relume Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relume, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Relume
provider_slug: relume
slug: relume-domain-security
source_filename: relume-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: relume.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 08:04:32 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: relume.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/relume/security/relume-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Website Builder
- Marketing
- No-code
---
