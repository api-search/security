---
api_specs:
- filename: keeptrack-openapi.yml
  format: yaml
  label: KeepTrack
  slug: keeptrack
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keeptrack/refs/heads/main/openapi/keeptrack-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keeptrack.space
  spf: true
hosts:
- cert_expires: Sep 21 04:43:46 2026 GMT
  host: www.keeptrack.space
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 05:06:40 2026 GMT
  host: api.keeptrack.space
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keeptrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KeepTrack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KeepTrack
provider_slug: keeptrack
slug: keeptrack-domain-security
source_filename: keeptrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keeptrack.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 04:43:46 2026 GMT\n  hsts: false\n- host: api.keeptrack.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:06:40 2026 GMT\n  hsts: false\ndomains:\n- domain: keeptrack.space\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keeptrack/refs/heads/main/security/keeptrack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Satellites
- Space
---
