---
api_specs:
- filename: ksq-therapeutics-pages-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Pages API
  slug: ksq-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-pages-api-openapi.yml
- filename: ksq-therapeutics-media-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Media API
  slug: ksq-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-media-api-openapi.yml
- filename: ksq-therapeutics-search-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Search API
  slug: ksq-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-search-api-openapi.yml
- filename: ksq-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Discovery API
  slug: ksq-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-discovery-api-openapi.yml
- filename: ksq-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Taxonomy API
  slug: ksq-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-taxonomy-api-openapi.yml
- filename: ksq-therapeutics-posts-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Posts API
  slug: ksq-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-posts-api-openapi.yml
- filename: ksq-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics oEmbed API
  slug: ksq-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-oembed-api-openapi.yml
- filename: ksq-therapeutics-press-release-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Press Release API
  slug: ksq-therapeutics-press-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-press-release-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ksqtx.com
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
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: ksqtx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ksq Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KSQ Therapeutics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KSQ Therapeutics
provider_slug: ksq-therapeutics
slug: ksq-therapeutics-domain-security
source_filename: ksq-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ksqtx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: ksqtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/security/ksq-therapeutics-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- biotechnology
- life-sciences
- therapeutics
- oncology
- genomics
- crispr
- gene-editing
- cell-therapy
- clinical-stage
- functional-genomics
- content-api
---
