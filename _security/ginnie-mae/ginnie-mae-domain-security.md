---
api_specs:
- filename: ginnie-mae-block-content-api-openapi.yml
  format: yaml
  label: Ginnie Mae Block Content API
  slug: ginnie-mae-block-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-block-content-api-openapi.yml
- filename: ginnie-mae-disclosure-api-openapi.yml
  format: yaml
  label: Ginnie Mae Disclosure API
  slug: ginnie-mae-disclosure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-disclosure-api-openapi.yml
- filename: ginnie-mae-discovery-api-openapi.yml
  format: yaml
  label: Ginnie Mae Discovery API
  slug: ginnie-mae-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-discovery-api-openapi.yml
- filename: ginnie-mae-entity-subqueue-api-openapi.yml
  format: yaml
  label: Ginnie Mae Entity Subqueue API
  slug: ginnie-mae-entity-subqueue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-entity-subqueue-api-openapi.yml
- filename: ginnie-mae-faq-api-openapi.yml
  format: yaml
  label: Ginnie Mae FAQ API
  slug: ginnie-mae-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-faq-api-openapi.yml
- filename: ginnie-mae-file-api-openapi.yml
  format: yaml
  label: Ginnie Mae File API
  slug: ginnie-mae-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-file-api-openapi.yml
- filename: ginnie-mae-media-api-openapi.yml
  format: yaml
  label: Ginnie Mae Media API
  slug: ginnie-mae-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-media-api-openapi.yml
- filename: ginnie-mae-menu-api-openapi.yml
  format: yaml
  label: Ginnie Mae Menu API
  slug: ginnie-mae-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-menu-api-openapi.yml
- filename: ginnie-mae-menu-link-content-api-openapi.yml
  format: yaml
  label: Ginnie Mae Menu Link Content API
  slug: ginnie-mae-menu-link-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-menu-link-content-api-openapi.yml
- filename: ginnie-mae-newsroom-api-openapi.yml
  format: yaml
  label: Ginnie Mae Newsroom API
  slug: ginnie-mae-newsroom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-newsroom-api-openapi.yml
- filename: ginnie-mae-node-api-openapi.yml
  format: yaml
  label: Ginnie Mae Node API
  slug: ginnie-mae-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-node-api-openapi.yml
- filename: ginnie-mae-paragraph-api-openapi.yml
  format: yaml
  label: Ginnie Mae Paragraph API
  slug: ginnie-mae-paragraph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-paragraph-api-openapi.yml
- filename: ginnie-mae-search-api-openapi.yml
  format: yaml
  label: Ginnie Mae Search API
  slug: ginnie-mae-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-search-api-openapi.yml
- filename: ginnie-mae-site-content-api-openapi.yml
  format: yaml
  label: Ginnie Mae Site Content API
  slug: ginnie-mae-site-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-site-content-api-openapi.yml
- filename: ginnie-mae-taxonomy-term-api-openapi.yml
  format: yaml
  label: Ginnie Mae Taxonomy Term API
  slug: ginnie-mae-taxonomy-term-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-taxonomy-term-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ginniemae.gov
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: www.ginniemae.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ginnie Mae Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ginnie Mae, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ginnie Mae
provider_slug: ginnie-mae
slug: ginnie-mae-domain-security
source_filename: ginnie-mae-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ginniemae.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ginniemae.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/security/ginnie-mae-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Housing
- Mortgage
- Mortgage-Backed Securities
- Open Data
- Content
- JSON:API
---
