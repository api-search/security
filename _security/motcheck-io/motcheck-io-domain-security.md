---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: motcheck.io
  spf: true
hosts:
- cert_expires: Jan 23 04:12:55 2027 GMT
  host: motcheck.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MOT Car Check Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOT Car Check, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MOT Car Check
provider_slug: motcheck-io
slug: motcheck-io-domain-security
source_filename: motcheck-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motcheck.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 04:12:55 2027 GMT\n  hsts: false\ndomains:\n- domain: motcheck.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/motcheck-io/security/motcheck-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- MOT History
- Vehicle check
- Car Valuation
- HPI check
---
