---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: minispli.com
  spf: true
hosts:
- cert_expires: Jan 29 19:59:22 2027 GMT
  host: minispli.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Old West Minisplits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Old West Minisplits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Old West Minisplits
provider_slug: minispli-com
slug: minispli-com-domain-security
source_filename: minispli-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minispli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 19:59:22 2027 GMT\n  hsts: false\ndomains:\n- domain: minispli.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/minispli-com/security/minispli-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- HVAC
- Ductless
- Mini-split
- Austin
- Residential
---
