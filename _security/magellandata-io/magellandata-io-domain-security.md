---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magellandata.io
  spf: true
hosts:
- cert_expires: Apr 16 23:59:59 2027 GMT
  host: magellandata.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Magellan Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magellan Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Magellan Data
provider_slug: magellandata-io
slug: magellandata-io-domain-security
source_filename: magellandata-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magellandata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: magellandata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/magellandata-io/security/magellandata-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Ownership
- Artificial Intelligence
---
