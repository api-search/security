---
description: ''
domains:
- caa:
  - 0 issue "symantec.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amerigroup.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: amerigroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amerigroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amerigroup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amerigroup
provider_slug: amerigroup
slug: amerigroup-domain-security
source_filename: amerigroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amerigroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amerigroup.com\n  dnssec: false\n  caa:\n  - 0 issue \"symantec.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amerigroup/refs/heads/main/security/amerigroup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Insurance
- Medicaid
- Managed Care
- Healthcare
- Government Programs
- Georgia
- Elevance Health
---
