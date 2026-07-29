---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hedna.org
  spf: true
hosts:
- cert_expires: Oct  2 21:53:10 2026 GMT
  host: www.hedna.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hedna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HEDNA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HEDNA
provider_slug: hedna
slug: hedna-domain-security
source_filename: hedna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hedna.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:53:10 2026 GMT\n  hsts: false\ndomains:\n- domain: hedna.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hedna/refs/heads/main/security/hedna-domain-security.yml
summary_line: TLSv1.3
tags:
- Travel
- United States
- Hospitality
- Hotels
- Distribution
- Booking
- GDS
- Standards
- Trade Association
---
