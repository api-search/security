---
api_specs:
- filename: thoughtspot-rest-v2-openapi-original.json
  format: json
  label: ThoughtSpot Public REST API v2.0
  slug: thoughtspot-public-rest-api-v20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thoughtspot/refs/heads/main/openapi/thoughtspot-rest-v2-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thoughtspot.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thoughtspot.cloud
  spf: true
hosts:
- cert_expires: Oct  1 14:45:20 2026 GMT
  host: www.thoughtspot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 14:45:20 2026 GMT
  host: developers.thoughtspot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: my.thoughtspot.cloud
  https: false
kind: domain-security
layout: security
method: probed
name: Thoughtspot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThoughtSpot, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ThoughtSpot
provider_slug: thoughtspot
slug: thoughtspot-domain-security
source_filename: thoughtspot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thoughtspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:45:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.thoughtspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:45:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.thoughtspot.cloud\n  https: false\ndomains:\n- domain: thoughtspot.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: thoughtspot.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thoughtspot/refs/heads/main/security/thoughtspot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Software
- Analytics
- Business Intelligence
- Data
- Embedded Analytics
- Artificial Intelligence
- Agents
- REST API
---
