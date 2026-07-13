---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gatekeeperhq.com
  spf: true
hosts:
- cert_expires: Aug 22 05:56:47 2026 GMT
  host: www.gatekeeperhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 01:15:21 2026 GMT
  host: knowledge.gatekeeperhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: app.gatekeeperhq.com
  https: false
kind: domain-security
layout: security
method: probed
name: Gatekeeper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gatekeeper, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gatekeeper
provider_slug: gatekeeper
slug: gatekeeper-domain-security
source_filename: gatekeeper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gatekeeperhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 05:56:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: knowledge.gatekeeperhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:15:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.gatekeeperhq.com\n  https: false\ndomains:\n- domain: gatekeeperhq.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gatekeeper/refs/heads/main/security/gatekeeper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contract Management
- Contract Lifecycle Management
- Vendor Management
- Procurement
- Supplier Management
- Legal Tech
- Risk Management
- E-Signature
---
