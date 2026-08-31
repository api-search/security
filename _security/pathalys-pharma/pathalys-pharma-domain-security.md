---
api_specs:
- filename: pathalys-pharma-posts-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Posts API
  slug: pathalys-pharma-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-posts-api-openapi.yml
- filename: pathalys-pharma-pages-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Pages API
  slug: pathalys-pharma-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-pages-api-openapi.yml
- filename: pathalys-pharma-media-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Media API
  slug: pathalys-pharma-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-media-api-openapi.yml
- filename: pathalys-pharma-categories-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Categories API
  slug: pathalys-pharma-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-categories-api-openapi.yml
- filename: pathalys-pharma-comments-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Comments API
  slug: pathalys-pharma-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-comments-api-openapi.yml
- filename: pathalys-pharma-search-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Search API
  slug: pathalys-pharma-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-search-api-openapi.yml
- filename: pathalys-pharma-discovery-api-openapi.yml
  format: yaml
  label: Pathalys Pharma Discovery API
  slug: pathalys-pharma-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/openapi/pathalys-pharma-discovery-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pathalys.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Oct 15 19:24:07 2026 GMT
  host: pathalys.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pathalys Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pathalys Pharma, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Pathalys Pharma
provider_slug: pathalys-pharma
slug: pathalys-pharma-domain-security
source_filename: pathalys-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pathalys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:24:07 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: pathalys.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pathalys-pharma/refs/heads/main/security/pathalys-pharma-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- pharmaceuticals
- biotechnology
- nephrology
- chronic-kidney-disease
- clinical-trials
- life-sciences
- content-api
---
