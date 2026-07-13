---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "akamai.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: surescripts.com
  spf: true
hosts:
- cert_expires: Aug 18 21:51:27 2026 GMT
  host: surescripts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Surescripts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Surescripts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Surescripts
provider_slug: surescripts
slug: surescripts-domain-security
source_filename: surescripts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: surescripts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 21:51:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: surescripts.com\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"akamai.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surescripts/refs/heads/main/security/surescripts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- E-Prescribing
- Health Information Network
- NCPDP SCRIPT
- Medication History
- Prior Authorization
- Interoperability
- Gated
---
