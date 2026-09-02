---
api_specs:
- filename: leandata-availability-api-openapi.yml
  format: yaml
  label: LeanData 🗓️ Availability API
  slug: leandata-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-availability-api-openapi.yml
- filename: leandata-legacy-still-supported-api-openapi.yml
  format: yaml
  label: LeanData Legacy (still supported) API
  slug: leandata-legacy-still-supported-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-legacy-still-supported-api-openapi.yml
- filename: leandata-matching-api-openapi.yml
  format: yaml
  label: LeanData Matching API
  slug: leandata-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-matching-api-openapi.yml
- filename: leandata-meetings-create-api-openapi.yml
  format: yaml
  label: LeanData 📆 Meetings > Create API
  slug: leandata-meetings-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-meetings-create-api-openapi.yml
- filename: leandata-meetings-manage-api-openapi.yml
  format: yaml
  label: LeanData 📆 Meetings > Manage API
  slug: leandata-meetings-manage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-meetings-manage-api-openapi.yml
- filename: leandata-meetings-retrieve-api-openapi.yml
  format: yaml
  label: LeanData 📆 Meetings > Retrieve API
  slug: leandata-meetings-retrieve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-meetings-retrieve-api-openapi.yml
- filename: leandata-one-time-routing-api-openapi.yml
  format: yaml
  label: LeanData One Time Routing API
  slug: leandata-one-time-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-one-time-routing-api-openapi.yml
- filename: leandata-retrieve-routing-graphs-information-api-openapi.yml
  format: yaml
  label: LeanData Retrieve Routing Graphs Information API
  slug: leandata-retrieve-routing-graphs-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-retrieve-routing-graphs-information-api-openapi.yml
- filename: leandata-scheduling-inputs-api-openapi.yml
  format: yaml
  label: LeanData 🧠 Scheduling Inputs API
  slug: leandata-scheduling-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-scheduling-inputs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leandata.com
  spf: true
hosts:
- cert_expires: Sep 14 23:03:12 2026 GMT
  host: www.leandata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 17:27:27 2026 GMT
  host: docs.leandata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: api.leandata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leandata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeanData, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LeanData
provider_slug: leandata
slug: leandata-domain-security
source_filename: leandata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leandata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:03:12 2026 GMT\n  hsts: false\n- host: docs.leandata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 17:27:27 2026 GMT\n  hsts: null\n- host: api.leandata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: leandata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/security/leandata-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Revenue Operations
- Lead Routing
- Lead to Account Matching
- Salesforce
- Sales Engagement
- Sales Productivity
- Marketing Operations
- Scheduling
- Meeting Booking
- Account Based Marketing
- Buying Groups
- Signal Orchestration
- Go-To-Market
- CRM
- AppExchange
---
