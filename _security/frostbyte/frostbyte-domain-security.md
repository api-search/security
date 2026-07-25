---
api_specs:
- filename: frostbyte-agent-infrastructure-api-openapi.yml
  format: yaml
  label: Frostbyte Agent Infrastructure API
  slug: frostbyte-agent-infrastructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-agent-infrastructure-api-openapi.yml
- filename: frostbyte-communication-api-openapi.yml
  format: yaml
  label: Frostbyte Communication API
  slug: frostbyte-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-communication-api-openapi.yml
- filename: frostbyte-crypto-prices-api-openapi.yml
  format: yaml
  label: Frostbyte Crypto Prices API
  slug: frostbyte-crypto-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-crypto-prices-api-openapi.yml
- filename: frostbyte-data-analytics-api-openapi.yml
  format: yaml
  label: Frostbyte Data & Analytics API
  slug: frostbyte-data-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-data-analytics-api-openapi.yml
- filename: frostbyte-defi-crypto-api-openapi.yml
  format: yaml
  label: Frostbyte DeFi & Crypto API
  slug: frostbyte-defi-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-defi-crypto-api-openapi.yml
- filename: frostbyte-gaming-api-openapi.yml
  format: yaml
  label: Frostbyte Gaming API
  slug: frostbyte-gaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-gaming-api-openapi.yml
- filename: frostbyte-gateway-api-openapi.yml
  format: yaml
  label: Frostbyte Gateway API
  slug: frostbyte-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-gateway-api-openapi.yml
- filename: frostbyte-ip-geolocation-api-openapi.yml
  format: yaml
  label: Frostbyte IP Geolocation API
  slug: frostbyte-ip-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-ip-geolocation-api-openapi.yml
- filename: frostbyte-other-api-openapi.yml
  format: yaml
  label: Frostbyte Other API
  slug: frostbyte-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-other-api-openapi.yml
- filename: frostbyte-security-api-openapi.yml
  format: yaml
  label: Frostbyte Security API
  slug: frostbyte-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-security-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vercel.app
  spf: true
hosts:
- cert_expires: Sep 26 13:27:56 2026 GMT
  host: api-catalog-three.vercel.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 13:27:56 2026 GMT
  host: agent-gateway-kappa.vercel.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frostbyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frostbyte, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Frostbyte
provider_slug: frostbyte
slug: frostbyte-domain-security
source_filename: frostbyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-catalog-three.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:27:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: agent-gateway-kappa.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:27:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vercel.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/security/frostbyte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Utility APIs
- Geolocation
- Cryptocurrency
- Screenshots
- DNS
- Scraping
- AI Agents
---
