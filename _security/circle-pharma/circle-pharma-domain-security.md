---
api_specs:
- filename: circle-pharma-categories-api-openapi.yml
  format: yaml
  label: Circle Pharma Categories API
  slug: circle-pharma-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-categories-api-openapi.yml
- filename: circle-pharma-comments-api-openapi.yml
  format: yaml
  label: Circle Pharma Comments API
  slug: circle-pharma-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-comments-api-openapi.yml
- filename: circle-pharma-discovery-api-openapi.yml
  format: yaml
  label: Circle Pharma Discovery API
  slug: circle-pharma-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-discovery-api-openapi.yml
- filename: circle-pharma-events-api-openapi.yml
  format: yaml
  label: Circle Pharma Events API
  slug: circle-pharma-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-events-api-openapi.yml
- filename: circle-pharma-media-api-openapi.yml
  format: yaml
  label: Circle Pharma Media API
  slug: circle-pharma-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-media-api-openapi.yml
- filename: circle-pharma-pages-api-openapi.yml
  format: yaml
  label: Circle Pharma Pages API
  slug: circle-pharma-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-pages-api-openapi.yml
- filename: circle-pharma-posts-api-openapi.yml
  format: yaml
  label: Circle Pharma Posts API
  slug: circle-pharma-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-posts-api-openapi.yml
- filename: circle-pharma-search-api-openapi.yml
  format: yaml
  label: Circle Pharma Search API
  slug: circle-pharma-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-search-api-openapi.yml
- filename: circle-pharma-tags-api-openapi.yml
  format: yaml
  label: Circle Pharma Tags API
  slug: circle-pharma-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-tags-api-openapi.yml
- filename: circle-pharma-team-api-openapi.yml
  format: yaml
  label: Circle Pharma Team API
  slug: circle-pharma-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-team-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: circlepharma.com
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
- cert_expires: Sep  7 08:13:01 2026 GMT
  host: circlepharma.com
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
name: Circle Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circle Pharma, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Circle Pharma
provider_slug: circle-pharma
slug: circle-pharma-domain-security
source_filename: circle-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: circlepharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 08:13:01 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: circlepharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/security/circle-pharma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Drug Discovery
- Macrocycles
- Clinical Trials
- Life Sciences
- content-api
---
