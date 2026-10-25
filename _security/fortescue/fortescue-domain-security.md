---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fortescue.com
  spf: true
hosts:
- cert_expires: Dec  8 16:48:13 2026 GMT
  host: fortescue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fortescue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortescue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fortescue
provider_slug: fortescue
slug: fortescue-domain-security
source_filename: fortescue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fortescue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 16:48:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fortescue.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortescue/refs/heads/main/security/fortescue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mining
- Iron Ore
- Metals
- Energy
- Decarbonisation
- Green Hydrogen
- Australia
---
