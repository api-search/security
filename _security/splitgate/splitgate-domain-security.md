---
api_specs:
- filename: splitgate-matches-api-openapi.yml
  format: yaml
  label: Splitgate Matches API
  slug: splitgate-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitgate/refs/heads/main/openapi/splitgate-matches-api-openapi.yml
- filename: splitgate-players-api-openapi.yml
  format: yaml
  label: Splitgate Players API
  slug: splitgate-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitgate/refs/heads/main/openapi/splitgate-players-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: splitgate.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 1047games.com
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.splitgate.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.1047games.com
  https: false
kind: domain-security
layout: security
method: probed
name: Splitgate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Splitgate, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Splitgate
provider_slug: splitgate
slug: splitgate-domain-security
source_filename: splitgate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.splitgate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: false\n- host: api.1047games.com\n  https: false\ndomains:\n- domain: splitgate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: 1047games.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splitgate/refs/heads/main/security/splitgate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Video Games
- Esports
- Player Statistics
- Leaderboards
- Match Data
- Entertainment
---
