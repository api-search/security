---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: everysim.io
  spf: true
hosts:
- cert_expires: Aug 25 13:40:12 2026 GMT
  host: everysim.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Everysim Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EverySim Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EverySim Inc.
provider_slug: everysim-inc
slug: everysim-inc-domain-security
source_filename: everysim-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: everysim.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 13:40:12 2026 GMT\n  hsts: null\ndomains:\n- domain: everysim.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everysim-inc/refs/heads/main/security/everysim-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Authentication
- OpenID Connect
- OAuth 2.0
- Single Sign-On
- Identity
---
