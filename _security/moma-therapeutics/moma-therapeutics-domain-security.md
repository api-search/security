---
api_specs:
- filename: moma-therapeutics-posts-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Content Posts API
  slug: moma-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-posts-api-openapi.yml
- filename: moma-therapeutics-pages-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Content Pages API
  slug: moma-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-pages-api-openapi.yml
- filename: moma-therapeutics-team-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Team API
  slug: moma-therapeutics-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-team-api-openapi.yml
- filename: moma-therapeutics-media-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Media API
  slug: moma-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-media-api-openapi.yml
- filename: moma-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Taxonomy API
  slug: moma-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-taxonomy-api-openapi.yml
- filename: moma-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Discovery API
  slug: moma-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-discovery-api-openapi.yml
- filename: moma-therapeutics-search-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Search API
  slug: moma-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-search-api-openapi.yml
- filename: moma-therapeutics-comments-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Comments API
  slug: moma-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-comments-api-openapi.yml
- filename: moma-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics oEmbed API
  slug: moma-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-oembed-api-openapi.yml
- filename: moma-therapeutics-options-api-openapi.yml
  format: yaml
  label: MOMA Therapeutics Site Options API
  slug: moma-therapeutics-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/openapi/moma-therapeutics-options-api-openapi.yml
description: ''
domains:
- caa: []
  caa_note: No CAA record — any public CA may issue for this domain.
  dmarc: true
  dmarc_note: DMARC is published but the policy is p=none, which monitors without enforcing. Neither quarantine nor reject is applied to unauthenticated mail claiming momatx.com.
  dmarc_policy: none
  dnssec: false
  domain: momatx.com
  spf: true
hosts:
- cert_expires: Nov 10 13:24:53 2026 GMT
  host: momatx.com
  hsts: false
  hsts_note: No Strict-Transport-Security response header on the apex. HTTP requests redirect to HTTPS, but without HSTS a first request is still downgradeable.
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moma Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOMA Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MOMA Therapeutics
provider_slug: moma-therapeutics
slug: moma-therapeutics-domain-security
source_filename: moma-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the momatx.com host on 2026-08-26\nnote: >-\n  Scoped to the one host MOMA Therapeutics controls. The automated probe also resolved\n  developer.wordpress.org and www.advancedcustomfields.com because those appear as humanURL\n  values on the API entries — they are upstream specification references for the WordPress and\n  ACF REST contracts, not MOMA infrastructure, and have been removed so this artifact describes\n  only the provider's own posture.\nhosts:\n- host: momatx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 13:24:53 2026 GMT\n  hsts: false\n  hsts_note: >-\n    No Strict-Transport-Security response header on the apex. HTTP requests redirect to HTTPS,\n    but without HSTS a first request is still downgradeable.\ndomains:\n- domain: momatx.com\n  dnssec: false\n  caa: []\n  caa_note: No CAA record — any public CA may issue for this domain.\n  spf: true\n  dmarc: true\n\
  \  dmarc_policy: none\n  dmarc_note: >-\n    DMARC is published but the policy is p=none, which monitors without enforcing. Neither\n    quarantine nor reject is applied to unauthenticated mail claiming momatx.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moma-therapeutics/refs/heads/main/security/moma-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- biotechnology
- pharmaceuticals
- drug-discovery
- oncology
- precision-medicine
- life-sciences
- structural-biology
- machine-learning
- content-api
---
