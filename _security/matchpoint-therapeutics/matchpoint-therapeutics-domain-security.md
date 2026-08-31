---
api_specs:
- filename: matchpoint-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Comments API
  slug: matchpoint-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-comments-api-openapi.yml
- filename: matchpoint-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Discovery API
  slug: matchpoint-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-discovery-api-openapi.yml
- filename: matchpoint-therapeutics-media-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Media API
  slug: matchpoint-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-media-api-openapi.yml
- filename: matchpoint-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Oembed API
  slug: matchpoint-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-oembed-api-openapi.yml
- filename: matchpoint-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Pages API
  slug: matchpoint-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-pages-api-openapi.yml
- filename: matchpoint-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Posts API
  slug: matchpoint-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-posts-api-openapi.yml
- filename: matchpoint-therapeutics-search-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Search API
  slug: matchpoint-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-search-api-openapi.yml
- filename: matchpoint-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Taxonomy API
  slug: matchpoint-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-taxonomy-api-openapi.yml
- filename: matchpoint-therapeutics-team-api-openapi.yml
  format: yaml
  label: Matchpoint Therapeutics Team API
  slug: matchpoint-therapeutics-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/openapi/matchpoint-therapeutics-team-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: matchpointtx.com
  spf: true
- caa:
  - 0 iodef "mailto:caa@wordpress.org"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Nov 15 20:31:39 2026 GMT
  host: matchpointtx.com
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
name: Matchpoint Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matchpoint Therapeutics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Matchpoint Therapeutics
provider_slug: matchpoint-therapeutics
slug: matchpoint-therapeutics-domain-security
source_filename: matchpoint-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matchpointtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 20:31:39 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: matchpointtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matchpoint-therapeutics/refs/heads/main/security/matchpoint-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Immunology
- Covalent Chemistry
- Chemoproteomics
- Machine Learning
- Life Sciences
- content-api
---
