---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pahdolabs.com
  spf: true
hosts:
- cert_expires: Sep 24 23:25:41 2026 GMT
  host: pahdolabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pahdo Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pahdo Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pahdo Labs
provider_slug: pahdo-labs
slug: pahdo-labs-domain-security
source_filename: pahdo-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pahdolabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:25:41 2026 GMT\n  hsts: null\ndomains:\n- domain: pahdolabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pahdo-labs/refs/heads/main/security/pahdo-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Game Development
- Game Engine
- Godot
- Entertainment
- Consumer
- Open Source
---
