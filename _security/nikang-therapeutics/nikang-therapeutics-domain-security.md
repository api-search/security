---
api_specs:
- filename: nikang-therapeutics-posts-api-openapi.yml
  format: yaml
  label: NiKang Therapeutics Posts API
  slug: nikang-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/openapi/nikang-therapeutics-posts-api-openapi.yml
- filename: nikang-therapeutics-pages-api-openapi.yml
  format: yaml
  label: NiKang Therapeutics Pages API
  slug: nikang-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/openapi/nikang-therapeutics-pages-api-openapi.yml
- filename: nikang-therapeutics-team-api-openapi.yml
  format: yaml
  label: NiKang Therapeutics Team API
  slug: nikang-therapeutics-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/openapi/nikang-therapeutics-team-api-openapi.yml
- filename: nikang-therapeutics-media-api-openapi.yml
  format: yaml
  label: NiKang Therapeutics Media API
  slug: nikang-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/openapi/nikang-therapeutics-media-api-openapi.yml
- filename: nikang-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: NiKang Therapeutics Taxonomy API
  slug: nikang-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/openapi/nikang-therapeutics-taxonomy-api-openapi.yml
- filename: nikang-therapeutics-search-api-openapi.yml
  format: yaml
  label: NiKang Therapeutics Search API
  slug: nikang-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/openapi/nikang-therapeutics-search-api-openapi.yml
- filename: nikang-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: NiKang Therapeutics Discovery API
  slug: nikang-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/openapi/nikang-therapeutics-discovery-api-openapi.yml
- filename: nikang-therapeutics-comments-api-openapi.yml
  format: yaml
  label: NiKang Therapeutics Comments API
  slug: nikang-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/openapi/nikang-therapeutics-comments-api-openapi.yml
- filename: nikang-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: NiKang Therapeutics oEmbed API
  slug: nikang-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/openapi/nikang-therapeutics-oembed-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nikangtx.com
  spf: true
hosts:
- cert_expires: Nov  8 04:56:30 2026 GMT
  edge: Cloudflare (server header `cloudflare`, cf-ray present) in front of a WP Engine origin (x-powered-by header `WP Engine`).
  host: www.nikangtx.com
  hsts: false
  https: true
  notes: '/wp-json responses carry `x-content-type-options: nosniff` and `x-robots-tag: noindex`. No Strict-Transport-Security, no Content-Security-Policy and no Referrer-Policy header was returned on either the HTML root or the JSON API.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nikang Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NiKang Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NiKang Therapeutics
provider_slug: nikang-therapeutics
slug: nikang-therapeutics-domain-security
source_filename: nikang-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of the hosts NiKang Therapeutics controls, run 2026-08-26 by\n  0-working/probe-domain-security.py and then trimmed by hand. The tool also probed\n  developer.wordpress.org and oembed.com because those are the humanURL hosts on the API entries;\n  both were removed, because they are upstream specification/documentation hosts that NiKang does\n  not operate and their posture must not be credited to NiKang.\nnote: >-\n  www.nikangtx.com terminates TLS at Cloudflare in front of a WP Engine origin. HSTS is NOT set on\n  either the site HTML or the /wp-json responses, and no CAA record is published for nikangtx.com,\n  so any CA may issue for the zone. Email authentication is the strongest part of the posture:\n  SPF is published and DMARC is at policy `reject`. DNSSEC is not enabled on the zone.\nhosts:\n- host: www.nikangtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Nov  8 04:56:30\
  \ 2026 GMT'\n  hsts: false\n  edge: >-\n    Cloudflare (server header `cloudflare`, cf-ray present) in front of a WP Engine origin\n    (x-powered-by header `WP Engine`).\n  notes: >-\n    /wp-json responses carry `x-content-type-options: nosniff` and `x-robots-tag: noindex`. No\n    Strict-Transport-Security, no Content-Security-Policy and no Referrer-Policy header was\n    returned on either the HTML root or the JSON API.\ndomains:\n- domain: nikangtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/security/nikang-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Precision Medicine
- Drug Discovery
- Targeted Protein Degradation
- Clinical Trials
- Life Sciences
- content-api
---
