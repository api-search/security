---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lightsource.ai
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: lightsource.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightsource Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LightSource, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LightSource
provider_slug: lightsource
slug: lightsource-domain-security
source_filename: lightsource-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightsource.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lightsource.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightsource/refs/heads/main/security/lightsource-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Procurement
- Supply Chain
- Sourcing
- Direct Materials
- Manufacturing
- Artificial Intelligence
- Enterprise Software
---
