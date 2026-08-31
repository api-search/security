---
api_specs:
- filename: namely-comments-api-openapi.yml
  format: yaml
  label: Namely Comments API
  slug: namely-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-comments-api-openapi.yml
- filename: namely-company-info-api-openapi.yml
  format: yaml
  label: Namely Company Info API
  slug: namely-company-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-company-info-api-openapi.yml
- filename: namely-company-resources-api-openapi.yml
  format: yaml
  label: Namely Company Resources API
  slug: namely-company-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-company-resources-api-openapi.yml
- filename: namely-countries-api-openapi.yml
  format: yaml
  label: Namely Countries API
  slug: namely-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-countries-api-openapi.yml
- filename: namely-events-api-openapi.yml
  format: yaml
  label: Namely Events API
  slug: namely-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-events-api-openapi.yml
- filename: namely-groups-api-openapi.yml
  format: yaml
  label: Namely Groups API
  slug: namely-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-groups-api-openapi.yml
- filename: namely-groups-teams-api-openapi.yml
  format: yaml
  label: Namely Groups & Teams API
  slug: namely-groups-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-groups-teams-api-openapi.yml
- filename: namely-home-feed-api-openapi.yml
  format: yaml
  label: Namely Home Feed API
  slug: namely-home-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-home-feed-api-openapi.yml
- filename: namely-job-tier-api-openapi.yml
  format: yaml
  label: Namely Job Tier API
  slug: namely-job-tier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-job-tier-api-openapi.yml
- filename: namely-job-title-api-openapi.yml
  format: yaml
  label: Namely Job Title API
  slug: namely-job-title-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-job-title-api-openapi.yml
- filename: namely-jobs-info-api-openapi.yml
  format: yaml
  label: Namely Jobs Info API
  slug: namely-jobs-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-jobs-info-api-openapi.yml
- filename: namely-likes-api-openapi.yml
  format: yaml
  label: Namely Likes API
  slug: namely-likes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-likes-api-openapi.yml
- filename: namely-namely-system-info-api-openapi.yml
  format: yaml
  label: Namely Namely System Info API
  slug: namely-namely-system-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-namely-system-info-api-openapi.yml
- filename: namely-notifications-api-openapi.yml
  format: yaml
  label: Namely Notifications API
  slug: namely-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-notifications-api-openapi.yml
- filename: namely-profile-fields-api-openapi.yml
  format: yaml
  label: Namely Profile Fields API
  slug: namely-profile-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-profile-fields-api-openapi.yml
- filename: namely-profile-fields-sections-api-openapi.yml
  format: yaml
  label: Namely Profile Fields Sections API
  slug: namely-profile-fields-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-profile-fields-sections-api-openapi.yml
- filename: namely-profiles-api-openapi.yml
  format: yaml
  label: Namely Profiles API
  slug: namely-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-profiles-api-openapi.yml
- filename: namely-reports-api-openapi.yml
  format: yaml
  label: Namely Reports API
  slug: namely-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-reports-api-openapi.yml
- filename: namely-teams-api-openapi.yml
  format: yaml
  label: Namely Teams API
  slug: namely-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: namely.com
  spf: true
hosts:
- cert_expires: Sep 29 18:37:47 2026 GMT
  host: namely.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 04:06:44 2026 GMT
  host: developers.namely.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Namely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Namely, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Namely
provider_slug: namely
slug: namely-domain-security
source_filename: namely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:37:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.namely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 04:06:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: namely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/security/namely-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- hr
- human-capital-management
- payroll
- employee-data
- Onboarding
- Benefits
- applicant-tracking
- performance-management
- SCIM
- single-sign-on
- identity-provisioning
- workforce-management
---
