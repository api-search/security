---
api_specs:
- filename: misskey-openapi.json
  format: json
  label: Misskey API
  slug: misskey
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misskey/refs/heads/main/openapi/misskey-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: misskey-hub.net
  spf: false
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: misskey.io
  spf: true
hosts:
- cert_expires: Sep 15 23:37:20 2026 GMT
  host: misskey-hub.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 18:05:22 2026 GMT
  host: misskey.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Misskey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Misskey, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Misskey
provider_slug: misskey
slug: misskey-domain-security
source_filename: misskey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: misskey-hub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:37:20 2026 GMT\n  hsts: false\n- host: misskey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:05:22 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: misskey-hub.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: misskey.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/misskey/refs/heads/main/security/misskey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open-Source
- Social Networks
- Fediverse
- ActivityPub
- Decentralized
---
