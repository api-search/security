---
api_specs:
- filename: usace-cwms-data-openapi.yml
  format: yaml
  label: USACE CWMS Data API
  slug: usace-cwms-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-army-corps-of-engineers/refs/heads/main/openapi/usace-cwms-data-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: army.mil
  spf: true
hosts:
- cert_expires: Sep 30 16:46:59 2026 GMT
  host: cwms-data.usace.army.mil
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:15:30 2026 GMT
  host: nid.sec.usace.army.mil
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  3 14:09:16 2026 GMT
  host: www.usace.army.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Army Corps Of Engineers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Army Corps of Engineers, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Army Corps of Engineers
provider_slug: us-army-corps-of-engineers
slug: us-army-corps-of-engineers-domain-security
source_filename: us-army-corps-of-engineers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cwms-data.usace.army.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:46:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: nid.sec.usace.army.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:15:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.usace.army.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 14:09:16 2026 GMT\n  hsts: null\ndomains:\n- domain: army.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-army-corps-of-engineers/refs/heads/main/security/us-army-corps-of-engineers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Water Resources
- Federal Government
- Military Engineering
- Infrastructure
- Open Data
- Geospatial Data
---
