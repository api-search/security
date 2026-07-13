---
api_specs:
- filename: hpe-openapi.yml
  format: yaml
  label: HPE GreenLake API
  slug: greenlake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hpe/refs/heads/main/openapi/hpe-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hpe.com
  spf: true
hosts:
- cert_expires: Jul 29 23:59:59 2026 GMT
  host: www.hpe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 00:45:11 2026 GMT
  host: developer.greenlake.hpe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: global.api.greenlake.hpe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hpe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hewlett Packard Enterprise, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hewlett Packard Enterprise
provider_slug: hpe
slug: hpe-domain-security
source_filename: hpe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hpe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 23:59:59 2026 GMT\n  hsts: null\n- host: developer.greenlake.hpe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 00:45:11 2026 GMT\n  hsts: false\n- host: global.api.greenlake.hpe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hpe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hpe/refs/heads/main/security/hpe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- Edge to Cloud
- Infrastructure as a Service
- Compute
- Storage
- Networking
- Hybrid Cloud
- Enterprise IT
---
