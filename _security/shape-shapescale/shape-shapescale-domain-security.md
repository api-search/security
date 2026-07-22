---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shapescale.com
  spf: true
hosts:
- cert_expires: Oct  2 15:52:56 2026 GMT
  host: shapescale.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shape Shapescale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shape Shapescale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shape Shapescale
provider_slug: shape-shapescale
slug: shape-shapescale-domain-security
source_filename: shape-shapescale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shapescale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:52:56 2026 GMT\n  hsts: false\ndomains:\n- domain: shapescale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shape-shapescale/refs/heads/main/security/shape-shapescale-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Body Scanning
- 3D Scanning
- Fitness
- Health
- Consumer Hardware
- Body Composition
- Y Combinator
---
