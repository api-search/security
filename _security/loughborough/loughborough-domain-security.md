---
api_specs:
- filename: loughborough-altmetric-api-openapi.yml
  format: yaml
  label: Loughborough University altmetric API
  slug: loughborough-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-altmetric-api-openapi.yml
- filename: loughborough-articles-api-openapi.yml
  format: yaml
  label: Loughborough University articles API
  slug: loughborough-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-articles-api-openapi.yml
- filename: loughborough-authors-api-openapi.yml
  format: yaml
  label: Loughborough University authors API
  slug: loughborough-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-authors-api-openapi.yml
- filename: loughborough-collections-api-openapi.yml
  format: yaml
  label: Loughborough University collections API
  slug: loughborough-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-collections-api-openapi.yml
- filename: loughborough-institutions-api-openapi.yml
  format: yaml
  label: Loughborough University institutions API
  slug: loughborough-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-institutions-api-openapi.yml
- filename: loughborough-oauth-api-openapi.yml
  format: yaml
  label: Loughborough University oauth API
  slug: loughborough-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-oauth-api-openapi.yml
- filename: loughborough-other-api-openapi.yml
  format: yaml
  label: Loughborough University other API
  slug: loughborough-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-other-api-openapi.yml
- filename: loughborough-profiles-api-openapi.yml
  format: yaml
  label: Loughborough University profiles API
  slug: loughborough-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-profiles-api-openapi.yml
- filename: loughborough-projects-api-openapi.yml
  format: yaml
  label: Loughborough University projects API
  slug: loughborough-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-projects-api-openapi.yml
- filename: loughborough-symplectic-api-openapi.yml
  format: yaml
  label: Loughborough University symplectic API
  slug: loughborough-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-symplectic-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lboro.ac.uk
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "certainly.com"
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.lboro.ac.uk
  hsts: true
  hsts_max_age: 15552000
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
name: Loughborough Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loughborough University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Loughborough University
provider_slug: loughborough
slug: loughborough-domain-security
source_filename: loughborough-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lboro.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lboro.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/security/loughborough-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Research Data
- Open Access
- Repository
- Identity
---
