---
api_specs:
- filename: memo-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Posts API
  slug: memo-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-posts-api-openapi.yml
- filename: memo-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Pages API
  slug: memo-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-pages-api-openapi.yml
- filename: memo-therapeutics-media-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Media API
  slug: memo-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-media-api-openapi.yml
- filename: memo-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Taxonomy API
  slug: memo-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-taxonomy-api-openapi.yml
- filename: memo-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Comments API
  slug: memo-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-comments-api-openapi.yml
- filename: memo-therapeutics-search-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Search API
  slug: memo-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-search-api-openapi.yml
- filename: memo-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Discovery API
  slug: memo-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-discovery-api-openapi.yml
- filename: memo-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Memo Therapeutics oEmbed API
  slug: memo-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-oembed-api-openapi.yml
- filename: memo-therapeutics-navigation-api-openapi.yml
  format: yaml
  label: Memo Therapeutics Navigation API
  slug: memo-therapeutics-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/openapi/memo-therapeutics-navigation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: memo-therapeutics.com
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: memo-therapeutics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memo Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memo Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Memo Therapeutics
provider_slug: memo-therapeutics
slug: memo-therapeutics-domain-security
source_filename: memo-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  Scoped to the host Memo Therapeutics controls. The probe also walked\n  developer.wordpress.org and wordpress.org because the apis[].humanURL points at the\n  upstream WordPress REST handbook that defines the wp/v2 contract; those results\n  describe the WordPress Foundation's posture, not Memo Therapeutics', and have been\n  removed so they are not read as this company's.\nfindings:\n  - memo-therapeutics.com serves TLS 1.3 with a certificate valid to 2027-02-27 but sends\n    no Strict-Transport-Security header.\n  - No DNSSEC and no CAA record on memo-therapeutics.com.\n  - SPF and DMARC are both published; the DMARC policy is p=reject. Mail is on Microsoft 365\n    (MX memotherapeutics-com01b.mail.protection.outlook.com).\nhosts:\n- host: memo-therapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\n\
  domains:\n- domain: memo-therapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memo-therapeutics/refs/heads/main/security/memo-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- biotechnology
- pharmaceuticals
- antibody-therapeutics
- rare-disease
- nephrology
- transplantation
- virology
- oncology
- clinical-trials
- life-sciences
- switzerland
- content-api
---
