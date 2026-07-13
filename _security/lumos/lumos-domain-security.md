---
api_specs:
- filename: lumos-openapi.yml
  format: yaml
  label: Lumos REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lumos.com
  spf: true
hosts:
- cert_expires: Sep 11 20:44:01 2026 GMT
  host: www.lumos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 19:52:28 2026 GMT
  host: developers.lumos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: api.lumos.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lumos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lumos
provider_slug: lumos
slug: lumos-domain-security
source_filename: lumos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lumos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:44:01 2026 GMT\n  hsts: false\n- host: developers.lumos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:52:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lumos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lumos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/security/lumos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Management
- Access Reviews
- Deprovisioning
- Identity Governance
- Identity Platform
- Least Privilege
- Provisioning
- SaaS Management
- Shadow IT
---
