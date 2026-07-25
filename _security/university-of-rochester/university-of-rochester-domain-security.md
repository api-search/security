---
api_specs:
- filename: university-of-rochester-altmetric-api-openapi.yml
  format: yaml
  label: University of Rochester altmetric API
  slug: university-of-rochester-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/openapi/university-of-rochester-altmetric-api-openapi.yml
- filename: university-of-rochester-articles-api-openapi.yml
  format: yaml
  label: University of Rochester articles API
  slug: university-of-rochester-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/openapi/university-of-rochester-articles-api-openapi.yml
- filename: university-of-rochester-authors-api-openapi.yml
  format: yaml
  label: University of Rochester authors API
  slug: university-of-rochester-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/openapi/university-of-rochester-authors-api-openapi.yml
- filename: university-of-rochester-collections-api-openapi.yml
  format: yaml
  label: University of Rochester collections API
  slug: university-of-rochester-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/openapi/university-of-rochester-collections-api-openapi.yml
- filename: university-of-rochester-institutions-api-openapi.yml
  format: yaml
  label: University of Rochester institutions API
  slug: university-of-rochester-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/openapi/university-of-rochester-institutions-api-openapi.yml
- filename: university-of-rochester-oauth-api-openapi.yml
  format: yaml
  label: University of Rochester oauth API
  slug: university-of-rochester-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/openapi/university-of-rochester-oauth-api-openapi.yml
- filename: university-of-rochester-other-api-openapi.yml
  format: yaml
  label: University of Rochester other API
  slug: university-of-rochester-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/openapi/university-of-rochester-other-api-openapi.yml
- filename: university-of-rochester-profiles-api-openapi.yml
  format: yaml
  label: University of Rochester profiles API
  slug: university-of-rochester-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/openapi/university-of-rochester-profiles-api-openapi.yml
- filename: university-of-rochester-projects-api-openapi.yml
  format: yaml
  label: University of Rochester projects API
  slug: university-of-rochester-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/openapi/university-of-rochester-projects-api-openapi.yml
- filename: university-of-rochester-symplectic-api-openapi.yml
  format: yaml
  label: University of Rochester symplectic API
  slug: university-of-rochester-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/openapi/university-of-rochester-symplectic-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rochester.edu
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "harica.gr"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.rochester.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
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
name: University Of Rochester Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Rochester, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Rochester
provider_slug: university-of-rochester
slug: university-of-rochester-domain-security
source_filename: university-of-rochester-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rochester.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rochester.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-rochester/refs/heads/main/security/university-of-rochester-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Institutional Repository
- Open Data
- United States
---
