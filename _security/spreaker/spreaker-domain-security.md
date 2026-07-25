---
api_specs:
- filename: spreaker-advertising-api-openapi.yml
  format: yaml
  label: Spreaker Advertising API
  slug: spreaker-advertising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-advertising-api-openapi.yml
- filename: spreaker-episodes-api-openapi.yml
  format: yaml
  label: Spreaker Episodes API
  slug: spreaker-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-episodes-api-openapi.yml
- filename: spreaker-search-and-discovery-api-openapi.yml
  format: yaml
  label: Spreaker Search and Discovery API
  slug: spreaker-search-and-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-search-and-discovery-api-openapi.yml
- filename: spreaker-shows-api-openapi.yml
  format: yaml
  label: Spreaker Shows API
  slug: spreaker-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-shows-api-openapi.yml
- filename: spreaker-statistics-api-openapi.yml
  format: yaml
  label: Spreaker Statistics API
  slug: spreaker-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-statistics-api-openapi.yml
- filename: spreaker-users-api-openapi.yml
  format: yaml
  label: Spreaker Users API
  slug: spreaker-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "rapidssl.com"
  - 0 iodef "mailto:operations@spreaker.com"
  - 0 issue "Digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spreaker.com
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: www.spreaker.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: developers.spreaker.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: api.spreaker.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spreaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spreaker, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spreaker
provider_slug: spreaker
slug: spreaker-domain-security
source_filename: spreaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spreaker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\n- host: developers.spreaker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.spreaker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: spreaker.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"rapidssl.com\"\n  - 0 iodef \"mailto:operations@spreaker.com\"\n  - 0 issue \"Digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/security/spreaker-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Podcasting
- Podcast Hosting
- Audio
- Media
- Monetization
- Analytics
---
