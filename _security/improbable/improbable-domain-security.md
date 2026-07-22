---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: improbable.io
  spf: true
hosts:
- cert_expires: Sep 24 14:38:18 2026 GMT
  host: www.improbable.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Improbable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Improbable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Improbable
provider_slug: improbable
slug: improbable-domain-security
source_filename: improbable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.improbable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 14:38:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: improbable.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/improbable/refs/heads/main/security/improbable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Venture Builder
- Metaverse
- Gaming
- Simulation
- Multiplayer
- Web3
- Infrastructure
- SDK
- London
---
