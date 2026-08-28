---
api_specs:
- filename: leaf4life-pages-api-openapi.yml
  format: yaml
  label: LEAF4Life Content Pages API
  slug: leaf4life-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-pages-api-openapi.yml
- filename: leaf4life-media-api-openapi.yml
  format: yaml
  label: LEAF4Life Media API
  slug: leaf4life-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-media-api-openapi.yml
- filename: leaf4life-taxonomy-api-openapi.yml
  format: yaml
  label: LEAF4Life Taxonomy API
  slug: leaf4life-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-taxonomy-api-openapi.yml
- filename: leaf4life-discovery-api-openapi.yml
  format: yaml
  label: LEAF4Life API Discovery
  slug: leaf4life-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-discovery-api-openapi.yml
- filename: leaf4life-search-api-openapi.yml
  format: yaml
  label: LEAF4Life Search API
  slug: leaf4life-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-search-api-openapi.yml
- filename: leaf4life-users-api-openapi.yml
  format: yaml
  label: LEAF4Life Authors API
  slug: leaf4life-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-users-api-openapi.yml
- filename: leaf4life-posts-api-openapi.yml
  format: yaml
  label: LEAF4Life Posts and Comments API
  slug: leaf4life-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-posts-api-openapi.yml
- filename: leaf4life-oembed-api-openapi.yml
  format: yaml
  label: LEAF4Life oEmbed API
  slug: leaf4life-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/openapi/leaf4life-oembed-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leafforlife.com
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
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: leafforlife.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 08:42:07 2026 GMT
  host: oembed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leaf4Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LEAF4Life, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LEAF4Life
provider_slug: leaf4life
slug: leaf4life-domain-security
source_filename: leaf4life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leafforlife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\n- host: oembed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 08:42:07 2026 GMT\n  hsts: false\ndomains:\n- domain: leafforlife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaf4life/refs/heads/main/security/leaf4life-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Clinical Trials
- Oncology
- Critical Care
- Drug Development
- Life Sciences
- Rare Disease
- content-api
---
