---
api_specs:
- filename: dalcor-pharmaceuticals-categories-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Categories API
  slug: dalcor-pharmaceuticals-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-categories-api-openapi.yml
- filename: dalcor-pharmaceuticals-comments-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Comments API
  slug: dalcor-pharmaceuticals-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-comments-api-openapi.yml
- filename: dalcor-pharmaceuticals-discovery-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Discovery API
  slug: dalcor-pharmaceuticals-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-discovery-api-openapi.yml
- filename: dalcor-pharmaceuticals-media-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Media API
  slug: dalcor-pharmaceuticals-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-media-api-openapi.yml
- filename: dalcor-pharmaceuticals-pages-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Pages API
  slug: dalcor-pharmaceuticals-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-pages-api-openapi.yml
- filename: dalcor-pharmaceuticals-posts-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Posts API
  slug: dalcor-pharmaceuticals-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-posts-api-openapi.yml
- filename: dalcor-pharmaceuticals-search-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Search API
  slug: dalcor-pharmaceuticals-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dalcorpharma.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep 27 03:05:17 2026 GMT
  edge: cloudflare
  host: dalcorpharma.com
  hsts: true
  hsts_evidence: 'GET/HEAD https://dalcorpharma.com/ with a browser User-Agent, 2026-08-04 -> 200, strict-transport-security: max-age=31536000'
  hsts_includesubdomains: false
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  other_security_headers:
  - 'x-content-type-options: nosniff'
  - 'x-frame-options: DENY'
  - 'referrer-policy: no-referrer-when-downgrade'
  - 'permissions-policy: geolocation=(), autoplay=(), camera=(), gyroscope=(), magnetometer=(), microphone=(), payment=()'
  - 'content-security-policy: default-src https: ''unsafe-inline'' ''self'' data:;'
  - 'x-xss-protection: 1; mode=block'
  - 'x-download-options: noopen'
  - 'cross-origin-resource-policy: cross-origin'
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dalcor Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DalCor Pharmaceuticals, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DalCor Pharmaceuticals
provider_slug: dalcor-pharmaceuticals
slug: dalcor-pharmaceuticals-domain-security
source_filename: dalcor-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  dalcorpharma.com sits behind Cloudflare and answers a default/absent User-Agent with HTTP 403, so\n  the mechanical probe recorded hsts: null for the site host. A re-probe with a browser User-Agent\n  returned HTTP 200 with `strict-transport-security: max-age=31536000` on both GET and HEAD of the\n  site root — corrected below and recorded with its evidence. developer.wordpress.org is the\n  humanURL host (the upstream WordPress REST handbook), not a DalCor-operated host.\nhosts:\n- host: dalcorpharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:05:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_includesubdomains: false\n  hsts_preload: false\n  hsts_evidence: 'GET/HEAD https://dalcorpharma.com/ with a browser User-Agent, 2026-08-04 -> 200,\n    strict-transport-security: max-age=31536000'\n  edge: cloudflare\n  other_security_headers:\n\
  \  - 'x-content-type-options: nosniff'\n  - 'x-frame-options: DENY'\n  - 'referrer-policy: no-referrer-when-downgrade'\n  - 'permissions-policy: geolocation=(), autoplay=(), camera=(), gyroscope=(), magnetometer=(),\n    microphone=(), payment=()'\n  - 'content-security-policy: default-src https: ''unsafe-inline'' ''self'' data:;'\n  - 'x-xss-protection: 1; mode=block'\n  - 'x-download-options: noopen'\n  - 'cross-origin-resource-policy: cross-origin'\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: null\ndomains:\n- domain: dalcorpharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/security/dalcor-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- pharmaceuticals
- biotechnology
- cardiovascular
- precision-medicine
- pharmacogenomics
- clinical-trials
- life-sciences
- content-api
---
