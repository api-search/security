---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: openclaw.direct
  spf: true
hosts:
- cert_expires: Feb  4 06:08:08 2027 GMT
  host: openclaw.direct
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenClaw Direct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenClaw Direct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: OpenClaw Direct
provider_slug: openclaw-direct
slug: openclaw-direct-domain-security
source_filename: openclaw-direct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openclaw.direct\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 06:08:08 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: openclaw.direct\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/openclaw-direct/security/openclaw-direct-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Platform
- Managed Service
- OpenClaw
- Assistant
---
