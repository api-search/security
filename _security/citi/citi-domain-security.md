---
description: ''
domains:
- caa:
  - 128 issuewild ";"
  - 128 iodef "mailto:CAADNS@citi.com"
  - 128 issue "globalsign.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: citi.com
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: www.citi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: developer.citi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Citi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Citi
provider_slug: citi
slug: citi-domain-security
source_filename: citi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.citi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\n- host: developer.citi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: citi.com\n  dnssec: false\n  caa:\n  - 128 issuewild \";\"\n  - 128 iodef \"mailto:CAADNS@citi.com\"\n  - 128 issue \"globalsign.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/security/citi-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Banking
- Financial Services
- Open Banking
- Payments
- Treasury
---
