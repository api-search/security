---
api_specs:
- filename: canny-autopilot-api-openapi.yml
  format: yaml
  label: Canny Autopilot API
  slug: canny-autopilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-autopilot-api-openapi.yml
- filename: canny-boards-api-openapi.yml
  format: yaml
  label: Canny Boards API
  slug: canny-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-boards-api-openapi.yml
- filename: canny-categories-api-openapi.yml
  format: yaml
  label: Canny Categories API
  slug: canny-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-categories-api-openapi.yml
- filename: canny-changelogentries-api-openapi.yml
  format: yaml
  label: Canny ChangelogEntries API
  slug: canny-changelogentries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-changelogentries-api-openapi.yml
- filename: canny-comments-api-openapi.yml
  format: yaml
  label: Canny Comments API
  slug: canny-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-comments-api-openapi.yml
- filename: canny-companies-api-openapi.yml
  format: yaml
  label: Canny Companies API
  slug: canny-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-companies-api-openapi.yml
- filename: canny-groups-api-openapi.yml
  format: yaml
  label: Canny Groups API
  slug: canny-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-groups-api-openapi.yml
- filename: canny-ideas-api-openapi.yml
  format: yaml
  label: Canny Ideas API
  slug: canny-ideas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-ideas-api-openapi.yml
- filename: canny-insights-api-openapi.yml
  format: yaml
  label: Canny Insights API
  slug: canny-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-insights-api-openapi.yml
- filename: canny-opportunities-api-openapi.yml
  format: yaml
  label: Canny Opportunities API
  slug: canny-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-opportunities-api-openapi.yml
- filename: canny-posts-api-openapi.yml
  format: yaml
  label: Canny Posts API
  slug: canny-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-posts-api-openapi.yml
- filename: canny-statuschanges-api-openapi.yml
  format: yaml
  label: Canny StatusChanges API
  slug: canny-statuschanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-statuschanges-api-openapi.yml
- filename: canny-tags-api-openapi.yml
  format: yaml
  label: Canny Tags API
  slug: canny-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-tags-api-openapi.yml
- filename: canny-users-api-openapi.yml
  format: yaml
  label: Canny Users API
  slug: canny-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-users-api-openapi.yml
- filename: canny-votes-api-openapi.yml
  format: yaml
  label: Canny Votes API
  slug: canny-votes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-votes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: canny.io
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: canny.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: developers.canny.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canny Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canny, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Canny
provider_slug: canny
slug: canny-domain-security
source_filename: canny-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canny.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.canny.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: canny.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/security/canny-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Feedback
- Product Management
- Feature Requests
- Roadmap
- Changelog
- Voice of Customer
- SaaS
---
