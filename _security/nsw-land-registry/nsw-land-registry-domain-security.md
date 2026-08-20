---
description: ''
domains:
- caa:
  - 0 issue "www.digicert.com"
  - 0 issuewild ";"
  - 0 iodef "mailto:CAA.Record.Status@nswlrs.com.au"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: false
  dnssec: true
  domain: nswlrs.com.au
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: nswlrs.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: connect.nswlrs.com.au
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: online.nswlrs.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nsw Land Registry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NSW Land Registry Services, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: NSW Land Registry Services
provider_slug: nsw-land-registry
slug: nsw-land-registry-domain-security
source_filename: nsw-land-registry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nswlrs.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.nswlrs.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\n- host: online.nswlrs.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: nswlrs.com.au\n  dnssec: true\n  caa:\n  - 0 issue \"www.digicert.com\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:CAA.Record.Status@nswlrs.com.au\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nsw-land-registry/refs/heads/main/security/nsw-land-registry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Real-Estate
- Australia
- Land Registry
- Title
- Conveyancing
- Property Records
- Torrens Title
- eConveyancing
- Government
- Geospatial
- PropTech
---
