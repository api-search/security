---
api_specs:
- filename: blablacar-bus-api-openapi.yaml
  format: yaml
  label: BlaBlaCar Bus API
  slug: blablacar-bus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/openapi/blablacar-bus-api-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issue "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:dns-ops@comuto.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: blablacar.com
  spf: true
hosts:
- cert_expires: Aug  3 14:30:19 2026 GMT
  host: www.blablacar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: bus-api.blablacar.com
  https: false
kind: domain-security
layout: security
method: probed
name: Blablacar Bus Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlaBlaCar Bus API, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
slug: blablacar-bus-api-domain-security
source_filename: blablacar-bus-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blablacar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 14:30:19 2026 GMT\n  hsts: false\n- host: bus-api.blablacar.com\n  https: false\ndomains:\n- domain: blablacar.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:dns-ops@comuto.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/security/blablacar-bus-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
---
