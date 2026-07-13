---
api_specs:
- filename: limble-cmms-limble-api-v2.yaml
  format: yaml
  label: Limble API V2
  slug: limble-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limble-cmms/refs/heads/main/openapi/limble-cmms-limble-api-v2.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: limble.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: limblecmms.com
  spf: true
hosts:
- cert_expires: Aug 12 17:55:29 2026 GMT
  host: limble.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: help.limblecmms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 17:50:15 2026 GMT
  host: apidocs.limblecmms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Limble Cmms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Limble CMMS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Limble CMMS
provider_slug: limble-cmms
slug: limble-cmms-domain-security
source_filename: limble-cmms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: limble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 17:55:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.limblecmms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.limblecmms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 17:50:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: limble.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: limblecmms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limble-cmms/refs/heads/main/security/limble-cmms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMMS
- Maintenance Management
- Asset Management
- Manufacturing
- Facility Management
- Work Orders
---
