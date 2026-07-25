---
api_specs:
- filename: figshare-altmetric-api-openapi.yml
  format: yaml
  label: Figshare altmetric API
  slug: figshare-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/openapi/figshare-altmetric-api-openapi.yml
- filename: figshare-articles-api-openapi.yml
  format: yaml
  label: Figshare articles API
  slug: figshare-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/openapi/figshare-articles-api-openapi.yml
- filename: figshare-authors-api-openapi.yml
  format: yaml
  label: Figshare authors API
  slug: figshare-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/openapi/figshare-authors-api-openapi.yml
- filename: figshare-collections-api-openapi.yml
  format: yaml
  label: Figshare collections API
  slug: figshare-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/openapi/figshare-collections-api-openapi.yml
- filename: figshare-institutions-api-openapi.yml
  format: yaml
  label: Figshare institutions API
  slug: figshare-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/openapi/figshare-institutions-api-openapi.yml
- filename: figshare-oauth-api-openapi.yml
  format: yaml
  label: Figshare oauth API
  slug: figshare-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/openapi/figshare-oauth-api-openapi.yml
- filename: figshare-other-api-openapi.yml
  format: yaml
  label: Figshare other API
  slug: figshare-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/openapi/figshare-other-api-openapi.yml
- filename: figshare-profiles-api-openapi.yml
  format: yaml
  label: Figshare profiles API
  slug: figshare-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/openapi/figshare-profiles-api-openapi.yml
- filename: figshare-projects-api-openapi.yml
  format: yaml
  label: Figshare projects API
  slug: figshare-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/openapi/figshare-projects-api-openapi.yml
- filename: figshare-symplectic-api-openapi.yml
  format: yaml
  label: Figshare symplectic API
  slug: figshare-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/openapi/figshare-symplectic-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: figshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: docs.figshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.figshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Figshare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Figshare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Figshare
provider_slug: figshare
slug: figshare-domain-security
source_filename: figshare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: figshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: docs.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/security/figshare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Research Data
- Data Repository
- Open Science
- DOI
- Datasets
- Academic
- File Storage
- Open Access
---
