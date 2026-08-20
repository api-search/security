---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prospera.ca
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.prospera.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Prospera Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prospera Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prospera Credit Union
provider_slug: prospera-credit-union
slug: prospera-credit-union-domain-security
source_filename: prospera-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prospera.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prospera.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prospera-credit-union/refs/heads/main/security/prospera-credit-union-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Canada
- Credit Union
- Cooperative
- British Columbia
- Interac
- Open Banking
- Consumer-Driven Banking
- Data Aggregation
---
