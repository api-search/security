---
api_specs:
- filename: nortech-openapi-original.json
  format: json
  label: Nortech Cloud API
  slug: nortech-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nor.tech
  spf: true
hosts:
- cert_expires: Sep 30 06:36:09 2026 GMT
  host: api.apps.nor.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nortech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nortech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nortech
provider_slug: nortech
slug: nortech-domain-security
source_filename: nortech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.apps.nor.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:36:09 2026 GMT\n  hsts: false\ndomains:\n- domain: nor.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/security/nortech-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Industrial IoT
- IIoT
- Maritime
- Operational Data
- Time Series
- Sensors
- Data Infrastructure
---
