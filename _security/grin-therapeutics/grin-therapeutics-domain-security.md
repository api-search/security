---
api_specs:
- filename: grin-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Discovery API
  slug: grin-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-discovery-api-openapi.yml
- filename: grin-therapeutics-media-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Media API
  slug: grin-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-media-api-openapi.yml
- filename: grin-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Oembed API
  slug: grin-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-oembed-api-openapi.yml
- filename: grin-therapeutics-pages-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Pages API
  slug: grin-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-pages-api-openapi.yml
- filename: grin-therapeutics-posts-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Posts API
  slug: grin-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-posts-api-openapi.yml
- filename: grin-therapeutics-search-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Search API
  slug: grin-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-search-api-openapi.yml
- filename: grin-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Taxonomy API
  slug: grin-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-taxonomy-api-openapi.yml
- filename: grin-therapeutics-users-api-openapi.yml
  format: yaml
  label: GRIN Therapeutics Users API
  slug: grin-therapeutics-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/openapi/grin-therapeutics-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grintherapeutics.com
  spf: true
hosts:
- cdn: Fastly (X-Served-By / X-Cache response headers observed)
  cert_expires: Oct 14 07:52:08 2026 GMT
  host: grintherapeutics.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 300
  hsts_preload: false
  https: true
  server: nginx
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grin Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GRIN Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GRIN Therapeutics
provider_slug: grin-therapeutics
slug: grin-therapeutics-domain-security
source_filename: grin-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the grintherapeutics.com host and registrable domain\nnote: >-\n  Probed 2026-08-04 by the API Evangelist enrichment pipeline. Only GRIN Therapeutics' own host and\n  registrable domain are recorded. The apis.yml humanURL for the content API points at\n  developer.wordpress.org (the upstream WordPress REST handbook that documents the wp/v2 contract);\n  that host is not operated by GRIN Therapeutics and its posture is deliberately excluded so it is\n  not misattributed to this provider. HSTS is present but the max-age is 300 seconds — three orders\n  of magnitude below the one-year value HSTS preload requires — with no includeSubDomains and no\n  preload directive, so it provides only nominal downgrade protection. No CAA records and no DNSSEC\n  are published.\nhosts:\n- host: grintherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:52:08 2026 GMT\n  hsts: true\n  hsts_max_age:\
  \ 300\n  hsts_include_subdomains: false\n  hsts_preload: false\n  server: nginx\n  cdn: Fastly (X-Served-By / X-Cache response headers observed)\ndomains:\n- domain: grintherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nobservations:\n- No Content-Security-Policy header on the site root.\n- No X-Content-Type-Options, X-Frame-Options, Referrer-Policy or Permissions-Policy header on the site root.\n- No /.well-known/security.txt (RFC 9116) published — see well-known/grin-therapeutics-well-known.yml.\n- No api., developer., docs., status., trust. or mcp. subdomain resolves for grintherapeutics.com (NXDOMAIN on all six).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grin-therapeutics/refs/heads/main/security/grin-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Neuroscience
- Rare Disease
- Precision Medicine
- Clinical Trials
- Pediatrics
- Epilepsy
- Life Sciences
- content-api
---
