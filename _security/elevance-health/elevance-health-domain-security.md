---
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elevancehealth.com
  spf: true
- caa:
  - 0 issue "symantec.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anthem.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: www.elevancehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.anthem.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: patient360.anthem.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Elevance Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elevance Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Elevance Health
provider_slug: elevance-health
slug: elevance-health-domain-security
source_filename: elevance-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elevancehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.anthem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: patient360.anthem.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: elevancehealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: anthem.com\n  dnssec: false\n  caa:\n  - 0 issue \"symantec.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/security/elevance-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Healthcare
- Health Insurance
- FHIR
- Interoperability
---
