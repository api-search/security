---
api_specs:
- filename: enveda-biosciences-comments-api-openapi.yml
  format: yaml
  label: Enveda Comments API
  slug: enveda-biosciences-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-comments-api-openapi.yml
- filename: enveda-biosciences-discovery-api-openapi.yml
  format: yaml
  label: Enveda Discovery API
  slug: enveda-biosciences-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-discovery-api-openapi.yml
- filename: enveda-biosciences-issues-api-openapi.yml
  format: yaml
  label: Enveda Issues API
  slug: enveda-biosciences-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-issues-api-openapi.yml
- filename: enveda-biosciences-media-api-openapi.yml
  format: yaml
  label: Enveda Media API
  slug: enveda-biosciences-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-media-api-openapi.yml
- filename: enveda-biosciences-news-api-openapi.yml
  format: yaml
  label: Enveda News API
  slug: enveda-biosciences-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-news-api-openapi.yml
- filename: enveda-biosciences-pages-api-openapi.yml
  format: yaml
  label: Enveda Pages API
  slug: enveda-biosciences-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-pages-api-openapi.yml
- filename: enveda-biosciences-people-api-openapi.yml
  format: yaml
  label: Enveda People API
  slug: enveda-biosciences-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-people-api-openapi.yml
- filename: enveda-biosciences-posts-api-openapi.yml
  format: yaml
  label: Enveda Posts API
  slug: enveda-biosciences-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-posts-api-openapi.yml
- filename: enveda-biosciences-search-api-openapi.yml
  format: yaml
  label: Enveda Search API
  slug: enveda-biosciences-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-search-api-openapi.yml
- filename: enveda-biosciences-settings-api-openapi.yml
  format: yaml
  label: Enveda Settings API
  slug: enveda-biosciences-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-settings-api-openapi.yml
- filename: enveda-biosciences-taxonomy-api-openapi.yml
  format: yaml
  label: Enveda Taxonomy API
  slug: enveda-biosciences-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-taxonomy-api-openapi.yml
- filename: enveda-biosciences-trial-sites-api-openapi.yml
  format: yaml
  label: Enveda Trial Sites API
  slug: enveda-biosciences-trial-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-trial-sites-api-openapi.yml
- filename: enveda-biosciences-users-api-openapi.yml
  format: yaml
  label: Enveda Users API
  slug: enveda-biosciences-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: enveda.com
  spf: true
hosts:
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:18:23 2026 GMT
  host: enveda.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enveda Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enveda, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Enveda
provider_slug: enveda-biosciences
slug: enveda-biosciences-domain-security
source_filename: enveda-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n- host: enveda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:18:23 2026 GMT\n  hsts: null\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: enveda.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/security/enveda-biosciences-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Drug Discovery
- Life Sciences
- Artificial Intelligence
- Machine Learning
- Metabolomics
- Natural Products
- Pharmaceuticals
- Clinical Trials
- Research
- Content
---
