---
api_specs:
- filename: erasmus-university-rotterdam-altmetric-api-openapi.yml
  format: yaml
  label: Erasmus University Rotterdam altmetric API
  slug: erasmus-university-rotterdam-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-altmetric-api-openapi.yml
- filename: erasmus-university-rotterdam-articles-api-openapi.yml
  format: yaml
  label: Erasmus University Rotterdam articles API
  slug: erasmus-university-rotterdam-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-articles-api-openapi.yml
- filename: erasmus-university-rotterdam-authors-api-openapi.yml
  format: yaml
  label: Erasmus University Rotterdam authors API
  slug: erasmus-university-rotterdam-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-authors-api-openapi.yml
- filename: erasmus-university-rotterdam-collections-api-openapi.yml
  format: yaml
  label: Erasmus University Rotterdam collections API
  slug: erasmus-university-rotterdam-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-collections-api-openapi.yml
- filename: erasmus-university-rotterdam-institutions-api-openapi.yml
  format: yaml
  label: Erasmus University Rotterdam institutions API
  slug: erasmus-university-rotterdam-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-institutions-api-openapi.yml
- filename: erasmus-university-rotterdam-oauth-api-openapi.yml
  format: yaml
  label: Erasmus University Rotterdam oauth API
  slug: erasmus-university-rotterdam-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-oauth-api-openapi.yml
- filename: erasmus-university-rotterdam-other-api-openapi.yml
  format: yaml
  label: Erasmus University Rotterdam other API
  slug: erasmus-university-rotterdam-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-other-api-openapi.yml
- filename: erasmus-university-rotterdam-profiles-api-openapi.yml
  format: yaml
  label: Erasmus University Rotterdam profiles API
  slug: erasmus-university-rotterdam-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-profiles-api-openapi.yml
- filename: erasmus-university-rotterdam-projects-api-openapi.yml
  format: yaml
  label: Erasmus University Rotterdam projects API
  slug: erasmus-university-rotterdam-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-projects-api-openapi.yml
- filename: erasmus-university-rotterdam-symplectic-api-openapi.yml
  format: yaml
  label: Erasmus University Rotterdam symplectic API
  slug: erasmus-university-rotterdam-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-symplectic-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:cert@eur.nl"
  - 0 issue "sectigo.com"
  - 0 issue "harica.gr"
  - 0 issuewild "harica.gr"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: eur.nl
  spf: true
hosts:
- cert_expires: Nov  5 14:30:52 2026 GMT
  host: www.eur.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 10:47:50 2026 GMT
  host: repub.eur.nl
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 27 05:59:14 2026 GMT
  host: pure.eur.nl
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Erasmus University Rotterdam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Erasmus University Rotterdam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Erasmus University Rotterdam
provider_slug: erasmus-university-rotterdam
slug: erasmus-university-rotterdam-domain-security
source_filename: erasmus-university-rotterdam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eur.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 14:30:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: repub.eur.nl\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 10:47:50 2026 GMT\n  hsts: false\n- host: pure.eur.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 05:59:14 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: eur.nl\n  dnssec: true\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:cert@eur.nl\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issuewild \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/security/erasmus-university-rotterdam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Repository
- OAI-PMH
- Netherlands
---
