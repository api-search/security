---
api_specs:
- filename: monash-altmetric-api-openapi.yml
  format: yaml
  label: Monash University altmetric API
  slug: monash-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-altmetric-api-openapi.yml
- filename: monash-articles-api-openapi.yml
  format: yaml
  label: Monash University articles API
  slug: monash-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-articles-api-openapi.yml
- filename: monash-authors-api-openapi.yml
  format: yaml
  label: Monash University authors API
  slug: monash-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-authors-api-openapi.yml
- filename: monash-collections-api-openapi.yml
  format: yaml
  label: Monash University collections API
  slug: monash-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-collections-api-openapi.yml
- filename: monash-institutions-api-openapi.yml
  format: yaml
  label: Monash University institutions API
  slug: monash-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-institutions-api-openapi.yml
- filename: monash-oauth-api-openapi.yml
  format: yaml
  label: Monash University oauth API
  slug: monash-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-oauth-api-openapi.yml
- filename: monash-other-api-openapi.yml
  format: yaml
  label: Monash University other API
  slug: monash-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-other-api-openapi.yml
- filename: monash-profiles-api-openapi.yml
  format: yaml
  label: Monash University profiles API
  slug: monash-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-profiles-api-openapi.yml
- filename: monash-projects-api-openapi.yml
  format: yaml
  label: Monash University projects API
  slug: monash-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-projects-api-openapi.yml
- filename: monash-symplectic-api-openapi.yml
  format: yaml
  label: Monash University symplectic API
  slug: monash-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-symplectic-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:cert-request-l@monash.edu"
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: monash.edu
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "harica.gr"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.monash.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: monash.figshare.com
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
name: Monash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monash University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Monash University
provider_slug: monash
slug: monash-domain-security
source_filename: monash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monash.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\n- host: monash.figshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: monash.edu\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:cert-request-l@monash.edu\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"\
  certainly.com\"\n  - 0 issuewild \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/security/monash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Australia
---
