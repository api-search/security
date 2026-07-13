---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apishare.cloud
  spf: true
hosts:
- cert_expires: Sep 16 15:34:45 2026 GMT
  host: www.apishare.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apishare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ApiShare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ApiShare
provider_slug: apishare
slug: apishare-domain-security
source_filename: apishare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apishare.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:34:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apishare.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apishare/refs/heads/main/security/apishare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Governance
- API Lifecycle
- API Management
- Catalog
- Governance
- Internal Developer Platform
- Platform
---
