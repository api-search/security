---
api_specs:
- filename: goatcounter-exports-api-openapi.yml
  format: yaml
  label: GoatCounter Exports API
  slug: goatcounter-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-exports-api-openapi.yml
- filename: goatcounter-pageviews-api-openapi.yml
  format: yaml
  label: GoatCounter Pageviews API
  slug: goatcounter-pageviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-pageviews-api-openapi.yml
- filename: goatcounter-paths-api-openapi.yml
  format: yaml
  label: GoatCounter Paths API
  slug: goatcounter-paths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-paths-api-openapi.yml
- filename: goatcounter-sites-api-openapi.yml
  format: yaml
  label: GoatCounter Sites API
  slug: goatcounter-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-sites-api-openapi.yml
- filename: goatcounter-statistics-api-openapi.yml
  format: yaml
  label: GoatCounter Statistics API
  slug: goatcounter-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-statistics-api-openapi.yml
- filename: goatcounter-users-api-openapi.yml
  format: yaml
  label: GoatCounter Users API
  slug: goatcounter-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-users-api-openapi.yml
- filename: goatcounter-count-api-openapi.yml
  format: yaml
  label: GoatCounter Count API
  slug: goatcounter-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-count-api-openapi.yml
- filename: goatcounter-export-api-openapi.yml
  format: yaml
  label: GoatCounter Export API
  slug: goatcounter-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-export-api-openapi.yml
- filename: goatcounter-stats-api-openapi.yml
  format: yaml
  label: GoatCounter Stats API
  slug: goatcounter-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-stats-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: goatcounter.com
  spf: true
hosts:
- cert_expires: Sep 16 14:20:14 2026 GMT
  host: www.goatcounter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 14:20:45 2026 GMT
  host: goatcounter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goatcounter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoatCounter, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: GoatCounter
provider_slug: goatcounter
slug: goatcounter-domain-security
source_filename: goatcounter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goatcounter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:20:14 2026 GMT\n  hsts: null\n- host: goatcounter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:20:45 2026 GMT\n  hsts: null\ndomains:\n- domain: goatcounter.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/security/goatcounter-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Analytics
- Page Views
- Privacy
- Statistics
- Web Analytics
- Open-Source
- Self-Hosted
- Event
- Data Export
- Developer Tools
---
