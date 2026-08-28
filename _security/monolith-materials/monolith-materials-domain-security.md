---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: monolith-corp.com
  spf: true
hosts:
- cert_expires: Nov 17 22:42:23 2026 GMT
  host: monolith-corp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monolith Materials Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monolith Materials, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Monolith Materials
provider_slug: monolith-materials
slug: monolith-materials-domain-security
source_filename: monolith-materials-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monolith-corp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 22:42:23 2026 GMT\n  hsts: false\ndomains:\n- domain: monolith-corp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monolith-materials/refs/heads/main/security/monolith-materials-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advanced Materials
- Chemicals
- Manufacturing
- Clean Hydrogen
- Carbon Black
- Energy Transition
- Industrial
---
