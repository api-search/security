---
api_specs:
- filename: simplivity-omnistack-openapi-original.json
  format: json
  label: HPE OmniStack REST API
  slug: hpe-omnistack-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-omnistack-openapi-original.json
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
kind: domain-security
layout: security
method: probed
name: Simplivity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpliVity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SimpliVity
provider_slug: simplivity
slug: simplivity-domain-security
source_filename: simplivity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hpe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hpe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/security/simplivity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Big Data
- Hyperconverged Infrastructure
- Virtualization
- Backup
- Disaster Recovery
- Data Center
- Storage
- Cloud Infrastructure
- HPE
---
