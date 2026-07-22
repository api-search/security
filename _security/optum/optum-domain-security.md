---
description: ''
domains:
- caa:
  - 0 issuemail "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: optum.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.optum.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 08:12:37 2026 GMT
  host: developer.optum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 04:13:37 2026 GMT
  host: apigw.optum.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Optum
provider_slug: optum
slug: optum-domain-security
source_filename: optum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.optum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.optum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 08:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apigw.optum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 04:13:37 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: optum.com\n  dnssec: true\n  caa:\n  - 0 issuemail \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/security/optum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health Insurance
- Claims
- Eligibility
- FHIR
- Interoperability
- Pharmacy
- EDI
- X12
- Payments
- Prior Authorization
---
