---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aetna.com
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: www.aetna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aetna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aetna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aetna
provider_slug: aetna
slug: aetna-domain-security
source_filename: aetna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aetna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aetna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/security/aetna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health Insurance
- Healthcare
- FHIR
- Patient Access
- Provider Directory
- Fortune 100
---
