---
api_specs:
- filename: icon-aircraft-store-api-openapi.yml
  format: yaml
  label: Shop ICON Storefront API
  slug: icon-aircraft-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-store-api-openapi.yml
- filename: icon-aircraft-catalog-api-openapi.yml
  format: yaml
  label: ICON Aircraft Catalog API
  slug: icon-aircraft-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-catalog-api-openapi.yml
- filename: icon-aircraft-collections-api-openapi.yml
  format: yaml
  label: ICON Aircraft Collections API
  slug: icon-aircraft-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-collections-api-openapi.yml
- filename: icon-aircraft-discovery-api-openapi.yml
  format: yaml
  label: ICON Aircraft Discovery API
  slug: icon-aircraft-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-discovery-api-openapi.yml
- filename: icon-aircraft-media-api-openapi.yml
  format: yaml
  label: ICON Aircraft Media API
  slug: icon-aircraft-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-media-api-openapi.yml
- filename: icon-aircraft-pages-api-openapi.yml
  format: yaml
  label: ICON Aircraft Pages API
  slug: icon-aircraft-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-pages-api-openapi.yml
- filename: icon-aircraft-posts-api-openapi.yml
  format: yaml
  label: ICON Aircraft Posts API
  slug: icon-aircraft-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-posts-api-openapi.yml
- filename: icon-aircraft-search-api-openapi.yml
  format: yaml
  label: ICON Aircraft Search API
  slug: icon-aircraft-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-search-api-openapi.yml
- filename: icon-aircraft-taxonomy-api-openapi.yml
  format: yaml
  label: ICON Aircraft Taxonomy API
  slug: icon-aircraft-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iconaircraft.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myshopify.com
  spf: true
hosts:
- cert_expires: Sep 27 17:17:29 2026 GMT
  host: www.iconaircraft.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 04:25:33 2026 GMT
  host: store.iconaircraft.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 15:01:35 2026 GMT
  host: iconaircraft.myshopify.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Icon Aircraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ICON Aircraft, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ICON Aircraft
provider_slug: icon-aircraft
slug: icon-aircraft-domain-security
source_filename: icon-aircraft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iconaircraft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:17:29 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: store.iconaircraft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 04:25:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: iconaircraft.myshopify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: iconaircraft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: myshopify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/security/icon-aircraft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Aerospace
- Aviation
- Aircraft Manufacturing
- Light Sport Aircraft
- Seaplanes
- General Aviation
- Flight Training
- Manufacturing
- Consumer Products
- E-Commerce
- Content
- Agentic Commerce
---
