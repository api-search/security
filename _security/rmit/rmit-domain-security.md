---
api_specs:
- filename: rmit-altmetric-api-openapi.yml
  format: yaml
  label: RMIT University altmetric API
  slug: rmit-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-altmetric-api-openapi.yml
- filename: rmit-articles-api-openapi.yml
  format: yaml
  label: RMIT University articles API
  slug: rmit-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-articles-api-openapi.yml
- filename: rmit-authors-api-openapi.yml
  format: yaml
  label: RMIT University authors API
  slug: rmit-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-authors-api-openapi.yml
- filename: rmit-collections-api-openapi.yml
  format: yaml
  label: RMIT University collections API
  slug: rmit-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-collections-api-openapi.yml
- filename: rmit-institutions-api-openapi.yml
  format: yaml
  label: RMIT University institutions API
  slug: rmit-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-institutions-api-openapi.yml
- filename: rmit-oauth-api-openapi.yml
  format: yaml
  label: RMIT University oauth API
  slug: rmit-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-oauth-api-openapi.yml
- filename: rmit-other-api-openapi.yml
  format: yaml
  label: RMIT University other API
  slug: rmit-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-other-api-openapi.yml
- filename: rmit-profiles-api-openapi.yml
  format: yaml
  label: RMIT University profiles API
  slug: rmit-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-profiles-api-openapi.yml
- filename: rmit-projects-api-openapi.yml
  format: yaml
  label: RMIT University projects API
  slug: rmit-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-projects-api-openapi.yml
- filename: rmit-symplectic-api-openapi.yml
  format: yaml
  label: RMIT University symplectic API
  slug: rmit-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-symplectic-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rmit.edu.au
  spf: true
- caa:
  - 0 issuewild "harica.gr"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.rmit.edu.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: rmit.figshare.com
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
name: Rmit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RMIT University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RMIT University
provider_slug: rmit
slug: rmit-domain-security
source_filename: rmit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rmit.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rmit.figshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rmit.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"harica.gr\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/security/rmit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Australia
---
