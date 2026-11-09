---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentzia.dev
  spf: true
hosts:
- cert_expires: Nov 26 04:44:20 2026 GMT
  host: agentzia.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentzia Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morphologic AI Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Morphologic AI Inc.
provider_slug: agentzia-dev
slug: agentzia-dev-domain-security
source_filename: agentzia-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentzia.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 04:44:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentzia.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentzia-dev/security/agentzia-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Geo
- Product Testing
- Generative AI
- Analytics
- Company
---
