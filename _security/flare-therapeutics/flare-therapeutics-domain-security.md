---
api_specs:
- filename: flare-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Comments API
  slug: flare-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-comments-api-openapi.yml
- filename: flare-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Discovery API
  slug: flare-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-discovery-api-openapi.yml
- filename: flare-therapeutics-media-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Media API
  slug: flare-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-media-api-openapi.yml
- filename: flare-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Oembed API
  slug: flare-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-oembed-api-openapi.yml
- filename: flare-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Pages API
  slug: flare-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-pages-api-openapi.yml
- filename: flare-therapeutics-patterns-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Patterns API
  slug: flare-therapeutics-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-patterns-api-openapi.yml
- filename: flare-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Posts API
  slug: flare-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-posts-api-openapi.yml
- filename: flare-therapeutics-search-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Search API
  slug: flare-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-search-api-openapi.yml
- filename: flare-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Flare Therapeutics Taxonomy API
  slug: flare-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/openapi/flare-therapeutics-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flaretx.com
  spf: true
hosts:
- cert_expires: Oct 26 19:28:00 2026 GMT
  host: www.flaretx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flare Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flare Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flare Therapeutics
provider_slug: flare-therapeutics
slug: flare-therapeutics-domain-security
source_filename: flare-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  Probed by 0-working/probe-domain-security.py on 2026-08-12. Only hosts Flare Therapeutics controls\n  are recorded. The probe also walked developer.wordpress.org / wordpress.org because the content\n  API entry uses the upstream WordPress REST handbook as its humanURL; those rows were removed\n  because they describe the WordPress Foundation's posture, not Flare's, and leaving them in would\n  credit or debit this provider for a domain it does not own. flaretx.com serves HSTS with a\n  two-year max-age but publishes no DNSSEC and no CAA records.\nhosts:\n- host: www.flaretx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 19:28:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flaretx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flare-therapeutics/refs/heads/main/security/flare-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Precision Medicine
- transcription-factors
- Drug Discovery
- Clinical Trials
- Life Sciences
- content-api
---
