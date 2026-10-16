---
api_specs:
- filename: dealroom-api-openapi.yml
  format: yaml
  label: Dealroom API API
  slug: dealroom-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealroom/refs/heads/main/openapi/_original/dealroom-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dealroom.co
  spf: true
hosts:
- cert_expires: Dec 27 10:35:45 2026 GMT
  host: dealroom.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dealroom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dealroom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Dealroom
provider_slug: dealroom
slug: dealroom-domain-security
source_filename: dealroom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dealroom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 10:35:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dealroom.co\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealroom/refs/heads/main/security/dealroom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
