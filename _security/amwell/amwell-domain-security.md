---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amwell.com
  spf: true
hosts:
- cert_expires: Apr  4 18:20:29 2027 GMT
  host: www.amwell.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  4 18:20:29 2027 GMT
  host: developers.amwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 20:59:15 2026 GMT
  host: business.amwell.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amwell, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amwell
provider_slug: amwell
slug: amwell-domain-security
source_filename: amwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 18:20:29 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developers.amwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 18:20:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: business.amwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 20:59:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: amwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amwell/refs/heads/main/security/amwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United States
- Telehealth
- Virtual Care
- FHIR
- HL7
- Interoperability
- EHR
- SDK
---
