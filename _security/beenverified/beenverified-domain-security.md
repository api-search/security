---
api_specs:
- filename: beenverified-append-api-openapi.yml
  format: yaml
  label: Beenverified Append API
  slug: beenverified-append-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beenverified/refs/heads/main/openapi/beenverified-append-api-openapi.yml
- filename: beenverified-append-sandbox-api-openapi.yml
  format: yaml
  label: Beenverified Append Sandbox API
  slug: beenverified-append-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beenverified/refs/heads/main/openapi/beenverified-append-sandbox-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beenverified.com
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: www.beenverified.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beenverified Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beenverified, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beenverified
provider_slug: beenverified
slug: beenverified-domain-security
source_filename: beenverified-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beenverified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: beenverified.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beenverified/refs/heads/main/security/beenverified-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Background-Check
- People-Search
- Data-API
- Consumer-Services
---
