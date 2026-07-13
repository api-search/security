---
api_specs:
- filename: hud-fair-market-rents-openapi.yml
  format: yaml
  label: HUD User Fair Market Rents API
  slug: hud-user-fair-market-rents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-fair-market-rents-openapi.yml
- filename: hud-income-limits-openapi.yml
  format: yaml
  label: HUD User Income Limits API
  slug: hud-user-income-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-income-limits-openapi.yml
- filename: hud-usps-zip-code-crosswalk-openapi.yml
  format: yaml
  label: HUD User USPS ZIP Code Crosswalk API
  slug: hud-user-usps-zip-code-crosswalk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-usps-zip-code-crosswalk-openapi.yml
- filename: hud-chas-openapi.yml
  format: yaml
  label: HUD User CHAS API
  slug: hud-user-chas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-chas-openapi.yml
- filename: hud-housing-counselor-search-openapi.yml
  format: yaml
  label: HUD Housing Counselor Search API
  slug: hud-housing-counselor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-housing-counselor-search-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:admin@hud.gov"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hud.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: huduser.gov
  spf: true
hosts:
- cert_expires: Sep  7 14:57:29 2026 GMT
  host: www.hud.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  1 17:54:38 2026 GMT
  host: www.huduser.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: data.hud.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HUD - US Department of Housing and Urban Development, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HUD - US Department of Housing and Urban Development
provider_slug: hud
slug: hud-domain-security
source_filename: hud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hud.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:57:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.huduser.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 17:54:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.hud.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hud.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:admin@hud.gov\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: huduser.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/security/hud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Housing
- Government
- Fair Market Rent
- Mortgage
- Community Development
- Public Housing
- Section 8
- Income Limits
---
