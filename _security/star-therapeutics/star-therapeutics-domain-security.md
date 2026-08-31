---
api_specs:
- filename: star-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Star Therapeutics Comments API
  slug: star-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-comments-api-openapi.yml
- filename: star-therapeutics-custom-types-api-openapi.yml
  format: yaml
  label: Star Therapeutics Custom Types API
  slug: star-therapeutics-custom-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-custom-types-api-openapi.yml
- filename: star-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Star Therapeutics Discovery API
  slug: star-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-discovery-api-openapi.yml
- filename: star-therapeutics-media-api-openapi.yml
  format: yaml
  label: Star Therapeutics Media API
  slug: star-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-media-api-openapi.yml
- filename: star-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Star Therapeutics Oembed API
  slug: star-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-oembed-api-openapi.yml
- filename: star-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Star Therapeutics Pages API
  slug: star-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-pages-api-openapi.yml
- filename: star-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Star Therapeutics Posts API
  slug: star-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-posts-api-openapi.yml
- filename: star-therapeutics-search-api-openapi.yml
  format: yaml
  label: Star Therapeutics Search API
  slug: star-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-search-api-openapi.yml
- filename: star-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Star Therapeutics Taxonomy API
  slug: star-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/openapi/star-therapeutics-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: star-therapeutics.com
  nameservers:
  - ns59.domaincontrol.com
  - ns60.domaincontrol.com
  spf: true
hosts:
- cert_expires: Sep 30 09:32:46 2026 GMT
  host: star-therapeutics.com
  hsts: false
  http3: true
  http_to_https_redirect: 301
  https: true
  origin: WP Engine (x-powered-by response header observed)
  server: cloudflare
  tls_version: TLSv1.3
  www_redirect: 301 to apex
kind: domain-security
layout: security
method: probed
name: Star Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Star Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Star Therapeutics
provider_slug: star-therapeutics
slug: star-therapeutics-domain-security
source_filename: star-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the star-therapeutics.com host and registrable domain\nnote: >-\n  Probed 2026-08-05 by the API Evangelist enrichment pipeline. Only Star Therapeutics' own host and\n  registrable domain are recorded. The apis.yml humanURL for the content API points at\n  developer.wordpress.org (the upstream WordPress REST handbook that documents the wp/v2 contract);\n  that host is not operated by Star Therapeutics and its posture is deliberately excluded so it is\n  not misattributed to this provider. The site is hosted on WP Engine and fronted by Cloudflare.\n  HTTPS is enforced by redirect (http:// and www. both 301 to https://star-therapeutics.com/) but\n  no Strict-Transport-Security header is sent, so the redirect is the only downgrade protection.\n  No CAA records and no DNSSEC are published; DNS is delegated to GoDaddy (domaincontrol.com).\nhosts:\n- host: star-therapeutics.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Sep 30 09:32:46 2026 GMT\n  hsts: false\n  server: cloudflare\n  origin: WP Engine (x-powered-by response header observed)\n  http_to_https_redirect: 301\n  www_redirect: 301 to apex\n  http3: true\ndomains:\n- domain: star-therapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  nameservers:\n  - ns59.domaincontrol.com\n  - ns60.domaincontrol.com\nobservations:\n- >-\n  DMARC aggregate reporting is misconfigured. The published record is\n  \"v=DMARC1; p=none; rua=mailto:admin@star-therapeutisc.com; ruf=mailto:admin@star-therapeutics.com\"\n  — the rua (aggregate report) address is a transposed-letter typo of the company's own domain,\n  \"star-therapeutisc.com\", which has no nameservers and does not resolve. Aggregate DMARC reports\n  are therefore being sent to a non-existent domain and are silently lost, while the ruf (forensic)\n  address is spelled correctly. Combined with p=none this means the domain has neither\
  \ enforcement\n  nor working visibility.\n- No Strict-Transport-Security header on the site root.\n- No Content-Security-Policy header on the site root.\n- No X-Content-Type-Options, X-Frame-Options, Referrer-Policy or Permissions-Policy header on the site root.\n- >-\n  API responses under /wp-json do send x-content-type-options nosniff and x-robots-tag noindex, and\n  expose Access-Control-Expose-Headers for X-WP-Total, X-WP-TotalPages, Link, Jet-Query-Total and\n  Jet-Query-Pages.\n- No /.well-known/security.txt (RFC 9116) published — see well-known/star-therapeutics-well-known.yml.\n- >-\n  No api., developer., docs., status., trust., mcp., support. or portal. subdomain resolves for\n  star-therapeutics.com (NXDOMAIN on all eight).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/star-therapeutics/refs/heads/main/security/star-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- biotechnology
- pharmaceuticals
- hematology
- immunology
- rare-disease
- antibody-therapeutics
- clinical-trials
- life-sciences
- content-api
---
