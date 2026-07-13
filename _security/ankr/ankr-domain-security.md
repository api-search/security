---
api_specs:
- filename: ankr-rpc-service-openapi.yml
  format: yaml
  label: Ankr RPC Service (Node API)
  slug: ankr-rpc-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-rpc-service-openapi.yml
- filename: ankr-advanced-api-openapi.yml
  format: yaml
  label: Ankr Advanced API
  slug: ankr-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-advanced-api-openapi.yml
- filename: ankr-staking-api-openapi.yml
  format: yaml
  label: Ankr Liquid Staking API
  slug: ankr-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-staking-api-openapi.yml
- filename: ankr-automation-api-openapi.yml
  format: yaml
  label: Ankr Contract Automation API
  slug: ankr-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-automation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ankr.com
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: www.ankr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 17:50:31 2026 GMT
  host: rpc.ankr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 07:25:16 2026 GMT
  host: api.staking.ankr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ankr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ankr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ankr
provider_slug: ankr
slug: ankr-domain-security
source_filename: ankr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ankr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rpc.ankr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 17:50:31 2026 GMT\n  hsts: null\n- host: api.staking.ankr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:25:16 2026 GMT\n  hsts: null\ndomains:\n- domain: ankr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/security/ankr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
