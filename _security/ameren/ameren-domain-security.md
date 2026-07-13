---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 128 issuevmc "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ameren.com
  spf: true
hosts:
- cert_expires: Oct  7 19:19:23 2026 GMT
  host: www.ameren.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.ameren.com
  https: false
- cert_expires: Oct  7 19:19:23 2026 GMT
  host: anm.ameren.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ameren Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ameren, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ameren
provider_slug: ameren
slug: ameren-domain-security
source_filename: ameren-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ameren.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:19:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ameren.com\n  https: false\n- host: anm.ameren.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:19:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ameren.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 128 issuevmc \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ameren/refs/heads/main/security/ameren-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Utility
- Energy
- Electric
- Natural Gas
- Smart Grid
- Green Button
- Renewable Energy
- Fortune 500
---
