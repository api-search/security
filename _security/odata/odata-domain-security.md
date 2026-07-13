---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: odata.org
  spf: false
hosts:
- cert_expires: Dec 13 04:32:57 2026 GMT
  host: www.odata.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Odata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OData
provider_slug: odata
slug: odata-domain-security
source_filename: odata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.odata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 04:32:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: odata.org\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odata/refs/heads/main/security/odata-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- OASIS Standard
- OData
- Open Data Protocol
- Query Language
- RESTful APIs
---
