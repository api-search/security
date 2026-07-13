---
api_specs:
- filename: sportsbook-api-openapi.yml
  format: yaml
  label: Sportsbook API
  slug: sportsbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsbook-api/refs/heads/main/openapi/sportsbook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: sportsbookapi.com
  spf: true
hosts:
- cert_expires: Sep 28 07:28:31 2026 GMT
  host: sportsbookapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 11:22:51 2026 GMT
  host: api.sportsbookapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sportsbook Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sportsbook API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Sportsbook API
provider_slug: sportsbook-api
slug: sportsbook-api-domain-security
source_filename: sportsbook-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sportsbookapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:28:31 2026 GMT\n  hsts: false\n- host: api.sportsbookapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:22:51 2026 GMT\n  hsts: false\ndomains:\n- domain: sportsbookapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsbook-api/refs/heads/main/security/sportsbook-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Sports Betting
- Odds
- Sports Data
- Gambling
---
