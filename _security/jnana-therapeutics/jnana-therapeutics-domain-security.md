---
api_specs:
- filename: jnana-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Comments API
  slug: jnana-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-comments-api-openapi.yml
- filename: jnana-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Discovery API
  slug: jnana-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-discovery-api-openapi.yml
- filename: jnana-therapeutics-media-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Media API
  slug: jnana-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-media-api-openapi.yml
- filename: jnana-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Oembed API
  slug: jnana-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-oembed-api-openapi.yml
- filename: jnana-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Pages API
  slug: jnana-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-pages-api-openapi.yml
- filename: jnana-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Posts API
  slug: jnana-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-posts-api-openapi.yml
- filename: jnana-therapeutics-search-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Search API
  slug: jnana-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-search-api-openapi.yml
- filename: jnana-therapeutics-seo-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Seo API
  slug: jnana-therapeutics-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-seo-api-openapi.yml
- filename: jnana-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Taxonomy API
  slug: jnana-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-taxonomy-api-openapi.yml
- filename: jnana-therapeutics-team-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Team API
  slug: jnana-therapeutics-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-team-api-openapi.yml
- filename: jnana-therapeutics-theme-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Theme API
  slug: jnana-therapeutics-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-theme-api-openapi.yml
- filename: jnana-therapeutics-users-api-openapi.yml
  format: yaml
  label: Jnana Therapeutics Users API
  slug: jnana-therapeutics-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/openapi/jnana-therapeutics-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jnanatx.com
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
- cert_expires: Nov 12 14:34:44 2026 GMT
  host: www.jnanatx.com
  hsts: true
  hsts_max_age: 63072000
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
name: Jnana Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jnana Therapeutics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jnana Therapeutics
provider_slug: jnana-therapeutics
slug: jnana-therapeutics-domain-security
source_filename: jnana-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jnanatx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 14:34:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: jnanatx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jnana-therapeutics/refs/heads/main/security/jnana-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Chemoproteomics
- Rare Disease
- Immunology
- Life Sciences
- Clinical Trials
- content-api
---
