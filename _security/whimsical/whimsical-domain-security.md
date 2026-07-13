---
api_specs:
- filename: whimsical-openapi.yml
  format: yaml
  label: Whimsical API (Beta)
  slug: whimsical-api-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/openapi/whimsical-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: whimsical.com
  spf: true
hosts:
- cert_expires: Sep 14 16:57:49 2026 GMT
  host: whimsical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whimsical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whimsical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Whimsical
provider_slug: whimsical
slug: whimsical-domain-security
source_filename: whimsical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whimsical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:57:49 2026 GMT\n  hsts: false\ndomains:\n- domain: whimsical.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/security/whimsical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Collaboration
- Diagramming
- Flowcharts
- Wireframes
- Mind Maps
---
