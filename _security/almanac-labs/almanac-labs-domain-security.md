---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: almanac.io
  spf: true
hosts:
- cert_expires: Oct 14 12:51:07 2026 GMT
  host: almanac.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 12:51:07 2026 GMT
  host: help.almanac.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 12:51:07 2026 GMT
  host: api.almanac.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Almanac Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Almanac Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Almanac Labs
provider_slug: almanac-labs
slug: almanac-labs-domain-security
source_filename: almanac-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: almanac.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 12:51:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.almanac.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 12:51:07 2026 GMT\n  hsts: null\n- host: api.almanac.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 12:51:07 2026 GMT\n  hsts: null\ndomains:\n- domain: almanac.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/almanac-labs/refs/heads/main/security/almanac-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Documentation
- Knowledge Management
- Collaboration
- Wiki
- Productivity
- Workflow
---
