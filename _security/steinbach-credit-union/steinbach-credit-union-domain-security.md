---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mb.ca
  spf: false
hosts:
- cert_expires: Sep 26 16:42:40 2026 GMT
  host: scu.mb.ca
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Steinbach Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Steinbach Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Steinbach Credit Union
provider_slug: steinbach-credit-union
slug: steinbach-credit-union-domain-security
source_filename: steinbach-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scu.mb.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:42:40 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: mb.ca\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steinbach-credit-union/refs/heads/main/security/steinbach-credit-union-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Financial-Services
- Banking
- Canada
- Credit Union
- Cooperative
- Manitoba
- Interac
- Data Aggregation
- Open Banking
---
