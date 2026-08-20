---
api_specs:
- filename: wugen-comments-api-openapi.yml
  format: yaml
  label: Wugen Comments API
  slug: wugen-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-comments-api-openapi.yml
- filename: wugen-discovery-api-openapi.yml
  format: yaml
  label: Wugen Discovery API
  slug: wugen-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-discovery-api-openapi.yml
- filename: wugen-media-api-openapi.yml
  format: yaml
  label: Wugen Media API
  slug: wugen-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-media-api-openapi.yml
- filename: wugen-pages-api-openapi.yml
  format: yaml
  label: Wugen Pages API
  slug: wugen-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-pages-api-openapi.yml
- filename: wugen-posts-api-openapi.yml
  format: yaml
  label: Wugen Posts API
  slug: wugen-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-posts-api-openapi.yml
- filename: wugen-search-api-openapi.yml
  format: yaml
  label: Wugen Search API
  slug: wugen-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-search-api-openapi.yml
- filename: wugen-taxonomy-api-openapi.yml
  format: yaml
  label: Wugen Taxonomy API
  slug: wugen-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/openapi/wugen-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alloteratx.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wugen.com
  spf: true
hosts:
- cert_expires: Sep 10 22:59:46 2026 GMT
  host: alloteratx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 19:13:07 2026 GMT
  host: wugen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wugen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wugen, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wugen
provider_slug: wugen
slug: wugen-domain-security
source_filename: wugen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alloteratx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 22:59:46 2026 GMT\n  hsts: false\n- host: wugen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 19:13:07 2026 GMT\n  hsts: false\ndomains:\n- domain: alloteratx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wugen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/security/wugen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Cell Therapy
- Oncology
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Cart
- CRISPR
- Immunotherapy
- Research
- Content
---
