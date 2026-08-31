---
api_specs:
- filename: inflammatix-categories-api-openapi.yml
  format: yaml
  label: Inflammatix Categories API
  slug: inflammatix-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-categories-api-openapi.yml
- filename: inflammatix-comments-api-openapi.yml
  format: yaml
  label: Inflammatix Comments API
  slug: inflammatix-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-comments-api-openapi.yml
- filename: inflammatix-coursecategories-api-openapi.yml
  format: yaml
  label: Inflammatix Course Categories API
  slug: inflammatix-coursecategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-coursecategories-api-openapi.yml
- filename: inflammatix-courses-api-openapi.yml
  format: yaml
  label: Inflammatix Courses API
  slug: inflammatix-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-courses-api-openapi.yml
- filename: inflammatix-coursetags-api-openapi.yml
  format: yaml
  label: Inflammatix Course Tags API
  slug: inflammatix-coursetags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-coursetags-api-openapi.yml
- filename: inflammatix-lessons-api-openapi.yml
  format: yaml
  label: Inflammatix Lessons API
  slug: inflammatix-lessons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-lessons-api-openapi.yml
- filename: inflammatix-media-api-openapi.yml
  format: yaml
  label: Inflammatix Media API
  slug: inflammatix-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-media-api-openapi.yml
- filename: inflammatix-pages-api-openapi.yml
  format: yaml
  label: Inflammatix Pages API
  slug: inflammatix-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-pages-api-openapi.yml
- filename: inflammatix-posts-api-openapi.yml
  format: yaml
  label: Inflammatix Posts API
  slug: inflammatix-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-posts-api-openapi.yml
- filename: inflammatix-publicationcategories-api-openapi.yml
  format: yaml
  label: Inflammatix Publication Categories API
  slug: inflammatix-publicationcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-publicationcategories-api-openapi.yml
- filename: inflammatix-publications-api-openapi.yml
  format: yaml
  label: Inflammatix Publications API
  slug: inflammatix-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-publications-api-openapi.yml
- filename: inflammatix-quizzes-api-openapi.yml
  format: yaml
  label: Inflammatix Quizzes API
  slug: inflammatix-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-quizzes-api-openapi.yml
- filename: inflammatix-search-api-openapi.yml
  format: yaml
  label: Inflammatix Search API
  slug: inflammatix-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-search-api-openapi.yml
- filename: inflammatix-statuses-api-openapi.yml
  format: yaml
  label: Inflammatix Statuses API
  slug: inflammatix-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-statuses-api-openapi.yml
- filename: inflammatix-tags-api-openapi.yml
  format: yaml
  label: Inflammatix Tags API
  slug: inflammatix-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-tags-api-openapi.yml
- filename: inflammatix-taxonomies-api-openapi.yml
  format: yaml
  label: Inflammatix Taxonomies API
  slug: inflammatix-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-taxonomies-api-openapi.yml
- filename: inflammatix-types-api-openapi.yml
  format: yaml
  label: Inflammatix Types API
  slug: inflammatix-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-types-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inflammatix.com
  spf: true
hosts:
- cert_expires: Sep  9 12:19:51 2026 GMT
  host: inflammatix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 20:32:35 2026 GMT
  host: support.inflammatix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inflammatix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inflammatix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Inflammatix
provider_slug: inflammatix
slug: inflammatix-domain-security
source_filename: inflammatix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inflammatix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 12:19:51 2026 GMT\n  hsts: false\n- host: support.inflammatix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:32:35 2026 GMT\n  hsts: false\ndomains:\n- domain: inflammatix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/security/inflammatix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Medical Devices
- In Vitro Diagnostics
- Molecular Diagnostics
- Sepsis
- Machine-Learning
- Life Sciences
- Point of Care
- Content
---
