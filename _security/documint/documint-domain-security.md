---
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: documint.me
  spf: true
hosts:
- cert_expires: Sep 16 15:03:23 2026 GMT
  host: www.documint.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 22:51:36 2026 GMT
  host: documint.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 01:57:24 2026 GMT
  host: api.documint.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Documint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Documint, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Documint
provider_slug: documint
slug: documint-domain-security
source_filename: documint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.documint.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:03:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: documint.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 22:51:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.documint.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:57:24 2026 GMT\n  hsts: false\ndomains:\n- domain: documint.me\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/documint/refs/heads/main/security/documint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Generation
- PDF
- Templates
- API
- Workflow
- HubSpot
- Zapier
---
