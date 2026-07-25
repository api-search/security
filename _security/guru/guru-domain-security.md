---
api_specs:
- filename: guru-analytics-api-openapi.yml
  format: yaml
  label: Guru Analytics API
  slug: guru-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-analytics-api-openapi.yml
- filename: guru-announcements-api-openapi.yml
  format: yaml
  label: Guru Announcements API
  slug: guru-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-announcements-api-openapi.yml
- filename: guru-answers-api-openapi.yml
  format: yaml
  label: Guru Answers API
  slug: guru-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-answers-api-openapi.yml
- filename: guru-cardcomments-api-openapi.yml
  format: yaml
  label: Guru CardComments API
  slug: guru-cardcomments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-cardcomments-api-openapi.yml
- filename: guru-cards-api-openapi.yml
  format: yaml
  label: Guru Cards API
  slug: guru-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-cards-api-openapi.yml
- filename: guru-cardverifiers-api-openapi.yml
  format: yaml
  label: Guru CardVerifiers API
  slug: guru-cardverifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-cardverifiers-api-openapi.yml
- filename: guru-collections-api-openapi.yml
  format: yaml
  label: Guru Collections API
  slug: guru-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-collections-api-openapi.yml
- filename: guru-folders-api-openapi.yml
  format: yaml
  label: Guru Folders API
  slug: guru-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-folders-api-openapi.yml
- filename: guru-groups-api-openapi.yml
  format: yaml
  label: Guru Groups API
  slug: guru-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-groups-api-openapi.yml
- filename: guru-members-api-openapi.yml
  format: yaml
  label: Guru Members API
  slug: guru-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-members-api-openapi.yml
- filename: guru-people-api-openapi.yml
  format: yaml
  label: Guru People API
  slug: guru-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-people-api-openapi.yml
- filename: guru-search-api-openapi.yml
  format: yaml
  label: Guru Search API
  slug: guru-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-search-api-openapi.yml
- filename: guru-tags-api-openapi.yml
  format: yaml
  label: Guru Tags API
  slug: guru-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-tags-api-openapi.yml
- filename: guru-tasks-api-openapi.yml
  format: yaml
  label: Guru Tasks API
  slug: guru-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-tasks-api-openapi.yml
- filename: guru-templates-api-openapi.yml
  format: yaml
  label: Guru Templates API
  slug: guru-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-templates-api-openapi.yml
- filename: guru-ticketlinking-api-openapi.yml
  format: yaml
  label: Guru TicketLinking API
  slug: guru-ticketlinking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-ticketlinking-api-openapi.yml
- filename: guru-user-api-openapi.yml
  format: yaml
  label: Guru User API
  slug: guru-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getguru.com
  spf: true
hosts:
- cert_expires: Sep 29 22:19:48 2026 GMT
  host: www.getguru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:01:58 2026 GMT
  host: developer.getguru.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.getguru.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guru, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Guru
provider_slug: guru
slug: guru-domain-security
source_filename: guru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getguru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:19:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.getguru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:01:58 2026 GMT\n  hsts: null\n- host: api.getguru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getguru.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/security/guru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Management
- Enterprise Search
- AI Knowledge Base
- Internal Wiki
- Verified Knowledge
- Workplace Productivity
---
