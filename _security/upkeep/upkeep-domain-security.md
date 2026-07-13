---
api_specs:
- filename: upkeep-openapi.yml
  format: yaml
  label: UpKeep API
  slug: upkeep
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/openapi/upkeep-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: upkeep.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: onupkeep.com
  spf: true
hosts:
- cert_expires: Aug 20 04:44:00 2026 GMT
  host: upkeep.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: developers.onupkeep.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:00:22 2026 GMT
  host: api.onupkeep.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upkeep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UpKeep, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: UpKeep
provider_slug: upkeep
slug: upkeep-domain-security
source_filename: upkeep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upkeep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:44:00 2026 GMT\n  hsts: false\n- host: developers.onupkeep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: api.onupkeep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:00:22 2026 GMT\n  hsts: null\ndomains:\n- domain: upkeep.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: onupkeep.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upkeep/refs/heads/main/security/upkeep-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- CMMS
- Maintenance Management
- Asset Management
- Facility Management
- Work Orders
---
