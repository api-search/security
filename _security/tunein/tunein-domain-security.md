---
api_specs:
- filename: openapi.yml
  format: yaml
  label: TuneIn Streaming API (OPML/RadioTime)
  slug: tunein-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tunein/refs/heads/main/openapi.yml
- filename: openapi-air.yml
  format: yaml
  label: TuneIn AIR (Broadcaster) API
  slug: tunein-air-broadcaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tunein/refs/heads/main/openapi-air.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@tunein.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tunein.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: corehacked.com
  spf: true
hosts:
- cert_expires: Aug 21 17:43:38 2026 GMT
  host: tunein.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 12:31:41 2026 GMT
  host: tunein-api.corehacked.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: opml.radiotime.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tunein Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TuneIn, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TuneIn
provider_slug: tunein
slug: tunein-domain-security
source_filename: tunein-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tunein.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 17:43:38 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: tunein-api.corehacked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:31:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: opml.radiotime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tunein.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@tunein.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: corehacked.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tunein/refs/heads/main/security/tunein-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Radio
- Internet Radio
- Podcasts
- Streaming Audio
- Sports Audio
- News Audio
- Music
---
