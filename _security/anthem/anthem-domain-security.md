---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "symantec.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anthem.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.anthem.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: fhir.anthem.com
  https: false
kind: domain-security
layout: security
method: probed
name: Anthem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anthem, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anthem
provider_slug: anthem
slug: anthem-domain-security
source_filename: anthem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anthem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fhir.anthem.com\n  https: false\ndomains:\n- domain: anthem.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"symantec.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anthem/refs/heads/main/security/anthem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blue Cross Blue Shield
- FHIR
- Health Benefits
- Health Insurance
- Healthcare
- Interoperability
- Fortune 100
---
