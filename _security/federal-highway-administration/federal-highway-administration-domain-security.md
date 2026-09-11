---
api_specs:
- filename: federal-highway-administration-v2x-app-api-openapi.json
  format: json
  label: FHWA V2X App API
  slug: v2x-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-v2x-app-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dot.gov
  spf: false
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: highways.dot.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Federal Highway Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Highway Administration, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Federal Highway Administration
provider_slug: federal-highway-administration
slug: federal-highway-administration-domain-security
source_filename: federal-highway-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highways.dot.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dot.gov\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/security/federal-highway-administration-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal-Government
- Transportation
- Highways
- Bridges
- Connected-Vehicles
- V2X
- Open-Source
- Open-Data
---
