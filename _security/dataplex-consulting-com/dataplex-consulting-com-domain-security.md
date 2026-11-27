---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dataplex-consulting.com
  spf: true
hosts:
- cert_expires: Dec 11 13:11:57 2026 GMT
  host: dataplex-consulting.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dataplex Consulting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dataplex Consulting, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dataplex Consulting
provider_slug: dataplex-consulting-com
slug: dataplex-consulting-com-domain-security
source_filename: dataplex-consulting-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataplex-consulting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 13:11:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dataplex-consulting.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dataplex-consulting-com/security/dataplex-consulting-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Healthcare
- Analytics
- Cloud
---
