---
api_specs:
- filename: hbku-altmetric-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University altmetric API
  slug: hbku-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-altmetric-api-openapi.yml
- filename: hbku-articles-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University articles API
  slug: hbku-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-articles-api-openapi.yml
- filename: hbku-authors-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University authors API
  slug: hbku-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-authors-api-openapi.yml
- filename: hbku-collections-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University collections API
  slug: hbku-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-collections-api-openapi.yml
- filename: hbku-institutions-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University institutions API
  slug: hbku-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-institutions-api-openapi.yml
- filename: hbku-oauth-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University oauth API
  slug: hbku-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-oauth-api-openapi.yml
- filename: hbku-other-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University other API
  slug: hbku-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-other-api-openapi.yml
- filename: hbku-profiles-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University profiles API
  slug: hbku-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-profiles-api-openapi.yml
- filename: hbku-projects-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University projects API
  slug: hbku-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-projects-api-openapi.yml
- filename: hbku-symplectic-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University symplectic API
  slug: hbku-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-symplectic-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hbku.edu.qa
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Sep 30 09:20:22 2026 GMT
  host: www.hbku.edu.qa
  hsts: true
  hsts_max_age: 300
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
name: Hbku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hamad Bin Khalifa University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hamad Bin Khalifa University
provider_slug: hbku
slug: hbku-domain-security
source_filename: hbku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hbku.edu.qa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:20:22 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hbku.edu.qa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/security/hbku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- Qatar
- Middle East
---
