---
api_specs:
- filename: xpansiv-connect-openapi.yml
  format: yaml
  label: Xpansiv Connect API
  slug: xpansiv-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-connect-openapi.yml
- filename: xpansiv-managed-solutions-openapi.yml
  format: yaml
  label: Xpansiv Managed Solutions API
  slug: xpansiv-managed-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-managed-solutions-openapi.yml
- filename: xpansiv-nar-registry-client-openapi.yml
  format: yaml
  label: NAR Registry Client API
  slug: xpansiv-nar-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-nar-registry-client-openapi.yml
- filename: xpansiv-tigr-registry-client-openapi.yml
  format: yaml
  label: TIGRS Registry Client API
  slug: xpansiv-tigr-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-tigr-registry-client-openapi.yml
- filename: xpansiv-optimal-system-openapi.yml
  format: yaml
  label: Xpansiv Optimal Outcomes APIs
  slug: xpansiv-optimal-outcomes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-optimal-system-openapi.yml
- filename: xpansiv-apx-power-markets-file-registry-openapi.yml
  format: yaml
  label: APX Power Markets File Registry API
  slug: xpansiv-apx-power-markets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-apx-power-markets-file-registry-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xpansiv.com
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: www.xpansiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 03:48:04 2026 GMT
  host: developer.xpansiv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 19:35:22 2026 GMT
  host: connect.xpansiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Xpansiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xpansiv, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xpansiv
provider_slug: xpansiv
slug: xpansiv-domain-security
source_filename: xpansiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xpansiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.xpansiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 03:48:04 2026 GMT\n  hsts: false\n- host: connect.xpansiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 19:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xpansiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/security/xpansiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Environmental Commodities
- Carbon Markets
- Renewable Energy Certificates
- Registries
- Market Data
- Trading
- Energy
- Sustainability
- Climate
---
