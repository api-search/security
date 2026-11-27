---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: hopi.co.uk
  spf: true
hosts:
- cert_expires: Jan  8 13:44:21 2027 GMT
  host: hopi.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hopi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hopi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Hopi
provider_slug: hopi-co-uk
slug: hopi-co-uk-domain-security
source_filename: hopi-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hopi.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 13:44:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hopi.co.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hopi-co-uk/security/hopi-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Tools
- Calculators
- Converters
- Utilities
---
