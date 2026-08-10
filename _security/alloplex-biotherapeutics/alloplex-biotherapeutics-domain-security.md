---
api_specs:
- filename: alloplex-biotherapeutics-discovery-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Discovery API
  slug: alloplex-biotherapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-discovery-api-openapi.yml
- filename: alloplex-biotherapeutics-media-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Media API
  slug: alloplex-biotherapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-media-api-openapi.yml
- filename: alloplex-biotherapeutics-oembed-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Oembed API
  slug: alloplex-biotherapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-oembed-api-openapi.yml
- filename: alloplex-biotherapeutics-pages-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Pages API
  slug: alloplex-biotherapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-pages-api-openapi.yml
- filename: alloplex-biotherapeutics-posts-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Posts API
  slug: alloplex-biotherapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-posts-api-openapi.yml
- filename: alloplex-biotherapeutics-search-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Search API
  slug: alloplex-biotherapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-search-api-openapi.yml
- filename: alloplex-biotherapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Alloplex Biotherapeutics Taxonomy API
  slug: alloplex-biotherapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/openapi/alloplex-biotherapeutics-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alloplexbio.com
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
- cert_expires: Oct  2 11:28:11 2026 GMT
  host: alloplexbio.com
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
name: Alloplex Biotherapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alloplex Biotherapeutics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alloplex Biotherapeutics
provider_slug: alloplex-biotherapeutics
slug: alloplex-biotherapeutics-domain-security
source_filename: alloplex-biotherapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alloplexbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:28:11 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: alloplexbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloplex-biotherapeutics/refs/heads/main/security/alloplex-biotherapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- biotechnology
- cell-therapy
- immunotherapy
- oncology
- cancer
- clinical-trials
- life-sciences
- drug-development
- autoimmunity
- content-api
---
