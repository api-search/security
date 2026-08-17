---
api_specs:
- filename: tps-engage-play-api-openapi.yml
  format: yaml
  label: TPS Engage Play API
  slug: tps-engage-play-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/openapi/tps-engage-play-api-openapi.yml
- filename: tps-engage-prefetch-api-openapi.yml
  format: yaml
  label: TPS Engage Prefetch API
  slug: tps-engage-prefetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/openapi/tps-engage-prefetch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: seeblindspot.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tpsengage.com
  spf: true
hosts:
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: seeblindspot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  checked: '2026-08-13'
  host: rtb.network.tpsengage.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'Corrected by hand on 2026-08-13. The automated probe recorded hsts: null because it reads headers only from a 2xx response, and every path on this host returns a 4xx/5xx to an anonymous caller. Observed directly on GET https://rtb.network.tpsengage.com/ (404) and on both documented operations: "Strict-Transport-Security: max-age=31536000; includeSubDomains".'
  https: true
  other_headers_observed:
  - 'Content-Security-Policy: default-src ''self''; …'
  - 'X-Content-Type-Options: nosniff'
  - 'X-Frame-Options: SAMEORIGIN'
  - 'Referrer-Policy: no-referrer'
  - 'Cross-Origin-Opener-Policy: same-origin'
  - 'Cross-Origin-Resource-Policy: same-origin'
  - 'Origin-Agent-Cluster: ?1'
  - 'X-Permitted-Cross-Domain-Policies: none'
  - 'access-control-allow-origin: *'
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tps Engage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TPS Engage, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TPS Engage
provider_slug: tps-engage
slug: tps-engage-domain-security
source_filename: tps-engage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seeblindspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rtb.network.tpsengage.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    Corrected by hand on 2026-08-13. The automated probe recorded hsts: null because\n    it reads headers only from a 2xx response, and every path on this host returns a\n    4xx/5xx to an anonymous caller. Observed directly on\n    GET https://rtb.network.tpsengage.com/ (404) and on both documented operations:\n    \"Strict-Transport-Security: max-age=31536000; includeSubDomains\".\n  other_headers_observed:\n  - 'Content-Security-Policy: default-src ''self''; …'\n  - 'X-Content-Type-Options: nosniff'\n  - 'X-Frame-Options:\
  \ SAMEORIGIN'\n  - 'Referrer-Policy: no-referrer'\n  - 'Cross-Origin-Opener-Policy: same-origin'\n  - 'Cross-Origin-Resource-Policy: same-origin'\n  - 'Origin-Agent-Cluster: ?1'\n  - 'X-Permitted-Cross-Domain-Policies: none'\n  - 'access-control-allow-origin: *'\n  checked: '2026-08-13'\ndomains:\n- domain: seeblindspot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tpsengage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/security/tps-engage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- DOOH
- Digital Billboards
- Programmatic Advertising
- Media Buying
- Out-of-Home
---
