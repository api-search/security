---
api_specs:
- filename: frostbyte-ip-geolocation-openapi.yml
  format: yaml
  label: Frostbyte IP Geolocation API
  slug: ip-geolocation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-ip-geolocation-openapi.yml
- filename: frostbyte-crypto-prices-openapi.yml
  format: yaml
  label: Frostbyte Crypto Prices API
  slug: crypto-prices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-crypto-prices-openapi.yml
- filename: frostbyte-screenshot-openapi.yml
  format: yaml
  label: Frostbyte Screenshot API
  slug: screenshot
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-screenshot-openapi.yml
- filename: frostbyte-dns-lookup-openapi.yml
  format: yaml
  label: Frostbyte DNS Lookup API
  slug: dns-lookup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-dns-lookup-openapi.yml
- filename: frostbyte-web-scraper-openapi.yml
  format: yaml
  label: Frostbyte Web Scraper API
  slug: web-scraper
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-web-scraper-openapi.yml
- filename: frostbyte-code-execution-openapi.yml
  format: yaml
  label: Frostbyte Code Execution API
  slug: code-execution
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-code-execution-openapi.yml
- filename: frostbyte-agent-gateway-openapi.yml
  format: yaml
  label: Frostbyte Agent Gateway (Full API)
  slug: agent-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-agent-gateway-openapi.yml
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
