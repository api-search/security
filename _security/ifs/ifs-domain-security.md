---
api_specs:
- filename: ifs-cloud-erp-openapi.yml
  format: yaml
  label: IFS Cloud ERP API
  slug: ifs-cloud-erp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-cloud-erp-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:noc@ifs.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ifs.com
  spf: true
hosts:
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: www.ifs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: api.ifs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ifs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IFS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IFS
provider_slug: ifs
slug: ifs-domain-security
source_filename: ifs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ifs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ifs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ifs.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:noc@ifs.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/security/ifs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Field Service
- Asset Management
- Manufacturing
- Energy
- Cloud
---
