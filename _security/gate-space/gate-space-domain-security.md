---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gate.space
  spf: true
hosts:
- cert_expires: Aug 31 23:16:18 2026 GMT
  host: gate.space
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gate Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GATE Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GATE Space
provider_slug: gate-space
slug: gate-space-domain-security
source_filename: gate-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gate.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:16:18 2026 GMT\n  hsts: false\ndomains:\n- domain: gate.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gate-space/refs/heads/main/security/gate-space-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aerospace
- Space
- Satellite
- Propulsion
- Space Mobility
- Hardware
- Defense
- Austria
---
