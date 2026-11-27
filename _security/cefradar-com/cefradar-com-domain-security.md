---
api_specs:
- filename: cefradar-com-account-api-openapi.yml
  format: yaml
  label: CEF Radar Account API
  slug: cefradar-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cefradar-com/openapi/cefradar-com-account-api-openapi.yml
- filename: cefradar-com-events-api-openapi.yml
  format: yaml
  label: CEF Radar Events API
  slug: cefradar-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cefradar-com/openapi/cefradar-com-events-api-openapi.yml
- filename: cefradar-com-funds-api-openapi.yml
  format: yaml
  label: CEF Radar Funds API
  slug: cefradar-com-funds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cefradar-com/openapi/cefradar-com-funds-api-openapi.yml
- filename: cefradar-com-investors-api-openapi.yml
  format: yaml
  label: CEF Radar Investors API
  slug: cefradar-com-investors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cefradar-com/openapi/cefradar-com-investors-api-openapi.yml
- filename: cefradar-com-search-api-openapi.yml
  format: yaml
  label: CEF Radar Search API
  slug: cefradar-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cefradar-com/openapi/cefradar-com-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cefradar.com
  spf: true
hosts:
- cert_expires: Dec 15 07:16:38 2026 GMT
  host: cefradar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CEF Radar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CEF Radar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CEF Radar
provider_slug: cefradar-com
slug: cefradar-com-domain-security
source_filename: cefradar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cefradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 07:16:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cefradar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cefradar-com/security/cefradar-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Closed‑end funds
- SEC Filings
- Investor alerts
- Fund Activity
- Buybacks
---
