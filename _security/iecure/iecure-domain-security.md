---
api_specs:
- filename: iecure-discovery-api-openapi.yml
  format: yaml
  label: iECURE Discovery API
  slug: iecure-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-discovery-api-openapi.yml
- filename: iecure-posts-api-openapi.yml
  format: yaml
  label: iECURE Posts API
  slug: iecure-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-posts-api-openapi.yml
- filename: iecure-pages-api-openapi.yml
  format: yaml
  label: iECURE Pages API
  slug: iecure-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-pages-api-openapi.yml
- filename: iecure-media-api-openapi.yml
  format: yaml
  label: iECURE Media API
  slug: iecure-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-media-api-openapi.yml
- filename: iecure-taxonomy-api-openapi.yml
  format: yaml
  label: iECURE Taxonomy API
  slug: iecure-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-taxonomy-api-openapi.yml
- filename: iecure-team-api-openapi.yml
  format: yaml
  label: iECURE Team API
  slug: iecure-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-team-api-openapi.yml
- filename: iecure-search-api-openapi.yml
  format: yaml
  label: iECURE Search API
  slug: iecure-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-search-api-openapi.yml
- filename: iecure-users-api-openapi.yml
  format: yaml
  label: iECURE Authors API
  slug: iecure-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-users-api-openapi.yml
- filename: iecure-comments-api-openapi.yml
  format: yaml
  label: iECURE Comments API
  slug: iecure-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-comments-api-openapi.yml
- filename: iecure-oembed-api-openapi.yml
  format: yaml
  label: iECURE oEmbed API
  slug: iecure-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/openapi/iecure-oembed-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iecure.com
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
- cert_expires: Oct 24 15:08:36 2026 GMT
  host: iecure.com
  hsts: false
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
name: Iecure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iECURE, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iECURE
provider_slug: iecure
slug: iecure-domain-security
source_filename: iecure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iecure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 15:08:36 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\n- host: oembed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 08:42:07 2026 GMT\n  hsts: false\ndomains:\n- domain: iecure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iecure/refs/heads/main/security/iecure-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Genetic Medicine
- Gene Editing
- Gene Therapy
- Rare Disease
- Clinical Trials
- Life Sciences
- Pharmaceuticals
- content-api
---
