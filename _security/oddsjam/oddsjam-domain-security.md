---
api_specs:
- filename: oddsjam-openapi.yml
  format: yaml
  label: OddsJam API
  slug: oddsjam
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/openapi/oddsjam-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oddsjam.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opticodds.com
  spf: false
hosts:
- cert_expires: Oct  7 14:16:58 2026 GMT
  host: oddsjam.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 10:52:20 2026 GMT
  host: api.opticodds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oddsjam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OddsJam, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OddsJam
provider_slug: oddsjam
slug: oddsjam-domain-security
source_filename: oddsjam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oddsjam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 14:16:58 2026 GMT\n  hsts: false\n- host: api.opticodds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 10:52:20 2026 GMT\n  hsts: null\ndomains:\n- domain: oddsjam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: opticodds.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oddsjam/refs/heads/main/security/oddsjam-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Odds
- Sports Betting
- Sportsbooks
---
