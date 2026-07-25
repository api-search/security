---
api_specs:
- filename: watchguard-accounts-api-openapi.yml
  format: yaml
  label: WatchGuard Accounts API
  slug: watchguard-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-accounts-api-openapi.yml
- filename: watchguard-activations-api-openapi.yml
  format: yaml
  label: WatchGuard Activations API
  slug: watchguard-activations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-activations-api-openapi.yml
- filename: watchguard-allocations-api-openapi.yml
  format: yaml
  label: WatchGuard Allocations API
  slug: watchguard-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-allocations-api-openapi.yml
- filename: watchguard-authorization-api-openapi.yml
  format: yaml
  label: WatchGuard Authorization API
  slug: watchguard-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-authorization-api-openapi.yml
- filename: watchguard-configurations-api-openapi.yml
  format: yaml
  label: WatchGuard Configurations API
  slug: watchguard-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-configurations-api-openapi.yml
- filename: watchguard-device-actions-api-openapi.yml
  format: yaml
  label: WatchGuard Device Actions API
  slug: watchguard-device-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-device-actions-api-openapi.yml
- filename: watchguard-devices-api-openapi.yml
  format: yaml
  label: WatchGuard Devices API
  slug: watchguard-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-devices-api-openapi.yml
- filename: watchguard-licenses-api-openapi.yml
  format: yaml
  label: WatchGuard Licenses API
  slug: watchguard-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-licenses-api-openapi.yml
- filename: watchguard-operators-api-openapi.yml
  format: yaml
  label: WatchGuard Operators API
  slug: watchguard-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-operators-api-openapi.yml
- filename: watchguard-risk-assessment-api-openapi.yml
  format: yaml
  label: WatchGuard Risk Assessment API
  slug: watchguard-risk-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-risk-assessment-api-openapi.yml
- filename: watchguard-security-events-api-openapi.yml
  format: yaml
  label: WatchGuard Security Events API
  slug: watchguard-security-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-security-events-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:itoperations@watchguard.com"
  - 0 issue "amazon.com"
  - 0 issue "cloudflare.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: watchguard.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.watchguard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.usa.cloud.watchguard.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.eu.cloud.watchguard.com
  https: false
kind: domain-security
layout: security
method: probed
name: Watchguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WatchGuard, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WatchGuard
provider_slug: watchguard
slug: watchguard-domain-security
source_filename: watchguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.watchguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usa.cloud.watchguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\n- host: api.eu.cloud.watchguard.com\n  https: false\ndomains:\n- domain: watchguard.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:itoperations@watchguard.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/security/watchguard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Security
- Endpoint Security
- Firewall
- MFA
- Network Security
- Zero Trust
---
