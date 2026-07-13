---
api_specs:
- filename: united-technologies-arinc-messaging-openapi.yml
  format: yaml
  label: Collins Aerospace ARINC Messaging API
  slug: arinc-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-technologies/refs/heads/main/openapi/united-technologies-arinc-messaging-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "sectigo.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rtx.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: collinsaerospace.com
  spf: true
hosts:
- cert_expires: Oct  1 10:20:19 2026 GMT
  host: www.rtx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:23:57 2026 GMT
  host: arinconline.collinsaerospace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.arinconline.collinsaerospace.com
  https: false
kind: domain-security
layout: security
method: probed
name: United Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Technologies, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: United Technologies
provider_slug: united-technologies
slug: united-technologies-domain-security
source_filename: united-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:20:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: arinconline.collinsaerospace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:23:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.arinconline.collinsaerospace.com\n  https: false\ndomains:\n- domain: rtx.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"sectigo.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: collinsaerospace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-technologies/refs/heads/main/security/united-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Aerospace
- Defense
- Aviation
- Manufacturing
- Connectivity
- Fortune 100
---
