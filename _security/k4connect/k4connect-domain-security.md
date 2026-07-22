---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "starfieldtech.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: k4connect.com
  spf: true
hosts:
- cert_expires: Sep  2 15:25:17 2026 GMT
  host: k4connect.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: K4Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for K4Connect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: K4Connect
provider_slug: k4connect
slug: k4connect-domain-security
source_filename: k4connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: k4connect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 15:25:17 2026 GMT\n  hsts: null\ndomains:\n- domain: k4connect.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/k4connect/refs/heads/main/security/k4connect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Digital Health
- Senior Living
- Aging Technology
- Integration Platform
- Data Interoperability
- Smart Home
- Resident Engagement
---
