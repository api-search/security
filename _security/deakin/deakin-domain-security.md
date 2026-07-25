---
api_specs:
- filename: deakin-altmetric-api-openapi.yml
  format: yaml
  label: Deakin University altmetric API
  slug: deakin-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-altmetric-api-openapi.yml
- filename: deakin-articles-api-openapi.yml
  format: yaml
  label: Deakin University articles API
  slug: deakin-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-articles-api-openapi.yml
- filename: deakin-authors-api-openapi.yml
  format: yaml
  label: Deakin University authors API
  slug: deakin-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-authors-api-openapi.yml
- filename: deakin-collections-api-openapi.yml
  format: yaml
  label: Deakin University collections API
  slug: deakin-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-collections-api-openapi.yml
- filename: deakin-institutions-api-openapi.yml
  format: yaml
  label: Deakin University institutions API
  slug: deakin-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-institutions-api-openapi.yml
- filename: deakin-oauth-api-openapi.yml
  format: yaml
  label: Deakin University oauth API
  slug: deakin-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-oauth-api-openapi.yml
- filename: deakin-other-api-openapi.yml
  format: yaml
  label: Deakin University other API
  slug: deakin-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-other-api-openapi.yml
- filename: deakin-profiles-api-openapi.yml
  format: yaml
  label: Deakin University profiles API
  slug: deakin-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-profiles-api-openapi.yml
- filename: deakin-projects-api-openapi.yml
  format: yaml
  label: Deakin University projects API
  slug: deakin-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-projects-api-openapi.yml
- filename: deakin-symplectic-api-openapi.yml
  format: yaml
  label: Deakin University symplectic API
  slug: deakin-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-symplectic-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "geotrust.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deakin.edu.au
  spf: true
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "certainly.com"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Aug 26 20:51:52 2026 GMT
  host: www.deakin.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: dro.deakin.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.figshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Deakin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deakin University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deakin University
provider_slug: deakin
slug: deakin-domain-security
source_filename: deakin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deakin.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:51:52 2026 GMT\n  hsts: false\n- host: dro.deakin.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deakin.edu.au\n  dnssec: false\n  caa:\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"\
  certainly.com\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/security/deakin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Australia
---
