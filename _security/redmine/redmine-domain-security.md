---
api_specs:
- filename: redmine-attachments-api-openapi.yml
  format: yaml
  label: Redmine Attachments API
  slug: redmine-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-attachments-api-openapi.yml
- filename: redmine-custom-fields-json-api-openapi.yml
  format: yaml
  label: Redmine Custom Fields.json API
  slug: redmine-custom-fields-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-custom-fields-json-api-openapi.yml
- filename: redmine-groups-json-api-openapi.yml
  format: yaml
  label: Redmine Groups.json API
  slug: redmine-groups-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-groups-json-api-openapi.yml
- filename: redmine-issue-statuses-json-api-openapi.yml
  format: yaml
  label: Redmine Issue Statuses.json API
  slug: redmine-issue-statuses-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-issue-statuses-json-api-openapi.yml
- filename: redmine-issues-api-openapi.yml
  format: yaml
  label: Redmine Issues API
  slug: redmine-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-issues-api-openapi.yml
- filename: redmine-issues-json-api-openapi.yml
  format: yaml
  label: Redmine Issues.json API
  slug: redmine-issues-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-issues-json-api-openapi.yml
- filename: redmine-my-api-openapi.yml
  format: yaml
  label: Redmine My API
  slug: redmine-my-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-my-api-openapi.yml
- filename: redmine-projects-api-openapi.yml
  format: yaml
  label: Redmine Projects API
  slug: redmine-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-projects-api-openapi.yml
- filename: redmine-projects-json-api-openapi.yml
  format: yaml
  label: Redmine Projects.json API
  slug: redmine-projects-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-projects-json-api-openapi.yml
- filename: redmine-roles-json-api-openapi.yml
  format: yaml
  label: Redmine Roles.json API
  slug: redmine-roles-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-roles-json-api-openapi.yml
- filename: redmine-time-entries-api-openapi.yml
  format: yaml
  label: Redmine Time Entries API
  slug: redmine-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-time-entries-api-openapi.yml
- filename: redmine-time-entries-json-api-openapi.yml
  format: yaml
  label: Redmine Time Entries.json API
  slug: redmine-time-entries-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-time-entries-json-api-openapi.yml
- filename: redmine-trackers-json-api-openapi.yml
  format: yaml
  label: Redmine Trackers.json API
  slug: redmine-trackers-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-trackers-json-api-openapi.yml
- filename: redmine-uploads-json-api-openapi.yml
  format: yaml
  label: Redmine Uploads.json API
  slug: redmine-uploads-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-uploads-json-api-openapi.yml
- filename: redmine-users-api-openapi.yml
  format: yaml
  label: Redmine Users API
  slug: redmine-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-users-api-openapi.yml
- filename: redmine-users-json-api-openapi.yml
  format: yaml
  label: Redmine Users.json API
  slug: redmine-users-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-users-json-api-openapi.yml
- filename: redmine-wiki-pages-json-api-openapi.yml
  format: yaml
  label: Redmine Wiki Pages.json API
  slug: redmine-wiki-pages-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-wiki-pages-json-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: redmine.org
  spf: true
hosts:
- cert_expires: Aug 12 03:03:32 2026 GMT
  host: www.redmine.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redmine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redmine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Redmine
provider_slug: redmine
slug: redmine-domain-security
source_filename: redmine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redmine.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 03:03:32 2026 GMT\n  hsts: false\ndomains:\n- domain: redmine.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/security/redmine-domain-security.yml
summary_line: TLSv1.3
tags:
- Project Management
- Issue Tracking
- Open Source
- Ruby on Rails
- Bug Tracking
- Time Tracking
---
