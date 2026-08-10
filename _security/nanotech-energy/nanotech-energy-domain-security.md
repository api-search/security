---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nanotechenergy.com
  spf: true
hosts:
- cert_expires: Sep 23 07:35:40 2026 GMT
  host: nanotechenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nanotech Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nanotech Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nanotech Energy
provider_slug: nanotech-energy
slug: nanotech-energy-domain-security
source_filename: nanotech-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nanotechenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:35:40 2026 GMT\n  hsts: false\ndomains:\n- domain: nanotechenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanotech-energy/refs/heads/main/security/nanotech-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Manufacturing
- Materials
- Graphene
- Nanotechnology
- Batteries
- Energy Storage
- Energy
---
