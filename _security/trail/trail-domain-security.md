---
api_specs:
- filename: trail_task_reports_v1.yaml
  format: yaml
  label: Trail Task Reports API
  slug: trail-task-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_task_reports_v1.yaml
- filename: trail_task_instances_v1.yaml
  format: yaml
  label: Trail Task Instances API
  slug: trail-task-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_task_instances_v1.yaml
- filename: trail_task_templates_v1.yaml
  format: yaml
  label: Trail Task Templates API
  slug: trail-task-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_task_templates_v1.yaml
- filename: trail_sites_v1.yaml
  format: yaml
  label: Trail Sites API
  slug: trail-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_sites_v1.yaml
- filename: trail_areas_v1.yaml
  format: yaml
  label: Trail Areas API
  slug: trail-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_areas_v1.yaml
- filename: trail_tags_v1.yaml
  format: yaml
  label: Trail Tags API
  slug: trail-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_tags_v1.yaml
- filename: trail_scores_v1.yaml
  format: yaml
  label: Trail Scores API
  slug: trail-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_scores_v1.yaml
- filename: trail_evo_api_v1.yaml
  format: yaml
  label: Trail Evo API
  slug: trail-evo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_evo_api_v1.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trailapp.com
  spf: true
hosts:
- cert_expires: Sep 26 21:14:49 2026 GMT
  host: trailapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:34:51 2026 GMT
  host: web.trailapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 00:09:36 2026 GMT
  host: us.trailapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trail, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trail
provider_slug: trail
slug: trail-domain-security
source_filename: trail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trailapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 21:14:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: web.trailapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:34:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: us.trailapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:09:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trailapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/security/trail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hospitality
- Checklists
- Task Management
- Compliance
- Food Safety
- Operations
---
