---
api_specs:
- filename: kriya-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Discovery API
  slug: kriya-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-discovery-api-openapi.yml
- filename: kriya-therapeutics-forms-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Forms API
  slug: kriya-therapeutics-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-forms-api-openapi.yml
- filename: kriya-therapeutics-media-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Media API
  slug: kriya-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-media-api-openapi.yml
- filename: kriya-therapeutics-news-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics News API
  slug: kriya-therapeutics-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-news-api-openapi.yml
- filename: kriya-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Oembed API
  slug: kriya-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-oembed-api-openapi.yml
- filename: kriya-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Pages API
  slug: kriya-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-pages-api-openapi.yml
- filename: kriya-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Posts API
  slug: kriya-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-posts-api-openapi.yml
- filename: kriya-therapeutics-search-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Search API
  slug: kriya-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-search-api-openapi.yml
- filename: kriya-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Taxonomy API
  slug: kriya-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-taxonomy-api-openapi.yml
- filename: kriya-therapeutics-team-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Team API
  slug: kriya-therapeutics-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-team-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: kriyatherapeutics.com
  spf: true
  spf_record: v=spf1 include:us._netblocks.mimecast.com include:spf.protection.outlook.com include:email.freshservice.com ~all
hosts:
- cdn: Cloudflare (cf-ray, cf-cache-status, cf-edge-cache=cache,platform=wordpress)
  cert_expires: Oct 18 08:21:55 2026 GMT
  host: kriyatherapeutics.com
  hsts: false
  hsts_include_subdomains: false
  hsts_max_age: null
  hsts_preload: false
  https: true
  origin: 'WP Engine (x-powered-by: WP Engine observed on REST responses)'
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kriya Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kriya Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kriya Therapeutics
provider_slug: kriya-therapeutics
slug: kriya-therapeutics-domain-security
source_filename: kriya-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the kriyatherapeutics.com host and registrable domain\nnote: >-\n  Probed 2026-08-04 by the API Evangelist enrichment pipeline. Only Kriya Therapeutics' own host and\n  registrable domain are recorded. The apis.yml humanURL for the content API points at\n  developer.wordpress.org (the upstream WordPress REST handbook that documents the wp/v2 contract);\n  that host is not operated by Kriya Therapeutics and its posture is deliberately excluded so it is\n  not misattributed to this provider. The site is served through Cloudflare in front of WP Engine.\n  No HSTS header is sent at all, so there is no downgrade protection and the domain is not\n  preload-eligible. SPF is published (Mimecast + Microsoft 365 + Freshservice) but there is no DMARC\n  record at _dmarc.kriyatherapeutics.com, so no policy governs what receivers do with unauthenticated\n  mail claiming to be from this domain. No CAA records and\
  \ no DNSSEC are published.\nhosts:\n- host: kriyatherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 08:21:55 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  hsts_include_subdomains: false\n  hsts_preload: false\n  server: cloudflare\n  origin: 'WP Engine (x-powered-by: WP Engine observed on REST responses)'\n  cdn: 'Cloudflare (cf-ray, cf-cache-status, cf-edge-cache=cache,platform=wordpress)'\ndomains:\n- domain: kriyatherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:us._netblocks.mimecast.com include:spf.protection.outlook.com include:email.freshservice.com ~all'\n  dmarc: false\n  dmarc_policy: null\nobservations:\n- No Strict-Transport-Security header on the site root or on the REST responses.\n- No Content-Security-Policy header on the site root.\n- No X-Frame-Options, Referrer-Policy or Permissions-Policy header on the site root.\n- 'X-Content-Type-Options: nosniff IS set on the /wp-json/ REST responses.'\n- No DMARC\
  \ record published for kriyatherapeutics.com, despite a valid SPF record being in place.\n- No /.well-known/security.txt (RFC 9116) published — see well-known/kriya-therapeutics-well-known.yml.\n- No api., developer., docs., status., trust., mcp. or portal. subdomain resolves for kriyatherapeutics.com (NXDOMAIN on all seven).\n- kriyatx.com resolves and 200-redirects to kriyatherapeutics.com; it serves the same WordPress deployment.\nexcluded_hosts:\n- host: developer.wordpress.org\n  reason: >-\n    Upstream WordPress REST handbook referenced as the API humanURL. Not operated by Kriya\n    Therapeutics; its TLS/DNS posture is not this provider's posture.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/security/kriya-therapeutics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Gene Therapy
- AAV
- Ophthalmology
- Metabolic Disease
- Neurology
- Life Sciences
- Clinical Trials
- Biomanufacturing
- content-api
---
