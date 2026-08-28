---
api_specs:
- filename: nusano-posts-api-openapi.yml
  format: yaml
  label: Nusano Posts API
  slug: posts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-posts-api-openapi.yml
- filename: nusano-pages-api-openapi.yml
  format: yaml
  label: Nusano Pages API
  slug: pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-pages-api-openapi.yml
- filename: nusano-media-api-openapi.yml
  format: yaml
  label: Nusano Media API
  slug: media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-media-api-openapi.yml
- filename: nusano-categories-api-openapi.yml
  format: yaml
  label: Nusano Categories API
  slug: categories
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-categories-api-openapi.yml
- filename: nusano-tags-api-openapi.yml
  format: yaml
  label: Nusano Tags API
  slug: tags
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-tags-api-openapi.yml
- filename: nusano-users-api-openapi.yml
  format: yaml
  label: Nusano Users API
  slug: users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-users-api-openapi.yml
- filename: nusano-comments-api-openapi.yml
  format: yaml
  label: Nusano Comments API
  slug: comments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-comments-api-openapi.yml
- filename: nusano-search-api-openapi.yml
  format: yaml
  label: Nusano Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-search-api-openapi.yml
- filename: nusano-discovery-api-openapi.yml
  format: yaml
  label: Nusano Discovery API
  slug: discovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-discovery-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nusano.com
  spf: true
hosts:
- cert_expires: Oct 10 00:13:08 2026 GMT
  host: nusano.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nusano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nusano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nusano
provider_slug: nusano
slug: nusano-domain-security
source_filename: nusano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nusano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:13:08 2026 GMT\n  hsts: false\ndomains:\n- domain: nusano.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/security/nusano-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Radioisotopes
- Nuclear Medicine
- Life Sciences
- Healthcare
- Oncology
- Radiopharmaceuticals
- Physics
- Advanced Manufacturing
- Nuclear Energy
- HALEU
- Critical Minerals
- Content
---
