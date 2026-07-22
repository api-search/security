---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: indriver.com
  spf: true
hosts:
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: indriver.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indrive Fka Indriver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InDrive (fka inDriver), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: InDrive (fka inDriver)
provider_slug: indrive-fka-indriver
slug: indrive-fka-indriver-domain-security
source_filename: indrive-fka-indriver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indriver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: indriver.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indrive-fka-indriver/refs/heads/main/security/indrive-fka-indriver-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mobility
- Ride-Hailing
- Transportation
- Delivery
- Super App
- Fintech
---
