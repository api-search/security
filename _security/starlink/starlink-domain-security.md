---
api_specs:
- filename: starlink-telemetry-asyncapi.yml
  format: yaml
  label: Starlink Telemetry Stream API
  slug: starlink-telemetry-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/asyncapi/starlink-telemetry-asyncapi.yml
- filename: starlink-account-api-openapi.yml
  format: yaml
  label: Starlink Account API
  slug: starlink-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-account-api-openapi.yml
- filename: starlink-addresses-api-openapi.yml
  format: yaml
  label: Starlink Addresses API
  slug: starlink-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-addresses-api-openapi.yml
- filename: starlink-billing-api-openapi.yml
  format: yaml
  label: Starlink Billing API
  slug: starlink-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-billing-api-openapi.yml
- filename: starlink-contacts-api-openapi.yml
  format: yaml
  label: Starlink Contacts API
  slug: starlink-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-contacts-api-openapi.yml
- filename: starlink-data-pools-api-openapi.yml
  format: yaml
  label: Starlink Data Pools API
  slug: starlink-data-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-data-pools-api-openapi.yml
- filename: starlink-flights-api-openapi.yml
  format: yaml
  label: Starlink Flights API
  slug: starlink-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-flights-api-openapi.yml
- filename: starlink-managed-accounts-api-openapi.yml
  format: yaml
  label: Starlink Managed Accounts API
  slug: starlink-managed-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-managed-accounts-api-openapi.yml
- filename: starlink-managed-api-openapi.yml
  format: yaml
  label: Starlink Managed API
  slug: starlink-managed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-managed-api-openapi.yml
- filename: starlink-mobile-api-openapi.yml
  format: yaml
  label: Starlink Mobile API
  slug: starlink-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-mobile-api-openapi.yml
- filename: starlink-routers-api-openapi.yml
  format: yaml
  label: Starlink Routers API
  slug: starlink-routers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-routers-api-openapi.yml
- filename: starlink-service-lines-api-openapi.yml
  format: yaml
  label: Starlink Service Lines API
  slug: starlink-service-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-service-lines-api-openapi.yml
- filename: starlink-user-terminals-api-openapi.yml
  format: yaml
  label: Starlink User Terminals API
  slug: starlink-user-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-user-terminals-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: starlink.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct  1 11:38:18 2026 GMT
  host: www.starlink.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: starlink.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 11:38:18 2026 GMT
  host: starlink.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starlink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starlink, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Starlink
provider_slug: starlink
slug: starlink-domain-security
source_filename: starlink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.starlink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:38:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: starlink.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: starlink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:38:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: starlink.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/security/starlink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- United States
- Satellite
- Broadband
- Non-Terrestrial Networks
- Connectivity
- Device Management
- Telemetry
- Aviation
- Maritime
- Enterprise
---
