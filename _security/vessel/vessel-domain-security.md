---
api_specs:
- filename: vessel-accounts-api-openapi.yml
  format: yaml
  label: Vessel Accounts API
  slug: vessel-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-accounts-api-openapi.yml
- filename: vessel-authentication-api-openapi.yml
  format: yaml
  label: Vessel Authentication API
  slug: vessel-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-authentication-api-openapi.yml
- filename: vessel-connections-api-openapi.yml
  format: yaml
  label: Vessel Connections API
  slug: vessel-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-connections-api-openapi.yml
- filename: vessel-contacts-api-openapi.yml
  format: yaml
  label: Vessel Contacts API
  slug: vessel-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-contacts-api-openapi.yml
- filename: vessel-deals-api-openapi.yml
  format: yaml
  label: Vessel Deals API
  slug: vessel-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-deals-api-openapi.yml
- filename: vessel-engagement-unifications-api-openapi.yml
  format: yaml
  label: Vessel Engagement Unifications API
  slug: vessel-engagement-unifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-engagement-unifications-api-openapi.yml
- filename: vessel-integrations-api-openapi.yml
  format: yaml
  label: Vessel Integrations API
  slug: vessel-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-integrations-api-openapi.yml
- filename: vessel-leads-api-openapi.yml
  format: yaml
  label: Vessel Leads API
  slug: vessel-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-leads-api-openapi.yml
- filename: vessel-notes-api-openapi.yml
  format: yaml
  label: Vessel Notes API
  slug: vessel-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-notes-api-openapi.yml
- filename: vessel-passthrough-api-openapi.yml
  format: yaml
  label: Vessel Passthrough API
  slug: vessel-passthrough-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-passthrough-api-openapi.yml
- filename: vessel-tasks-api-openapi.yml
  format: yaml
  label: Vessel Tasks API
  slug: vessel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-tasks-api-openapi.yml
- filename: vessel-users-api-openapi.yml
  format: yaml
  label: Vessel Users API
  slug: vessel-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-users-api-openapi.yml
- filename: vessel-webhooks-api-openapi.yml
  format: yaml
  label: Vessel Webhooks API
  slug: vessel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vessel.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vessel.land
  spf: true
hosts:
- cert_expires: Oct  1 06:58:09 2026 GMT
  host: www.vessel.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.vessel.land
  https: false
- cert_expires: Aug 16 11:23:53 2026 GMT
  host: api.vessel.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vessel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vessel, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vessel
provider_slug: vessel
slug: vessel-domain-security
source_filename: vessel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vessel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:58:09 2026 GMT\n  hsts: false\n- host: api.vessel.land\n  https: false\n- host: api.vessel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:23:53 2026 GMT\n  hsts: null\ndomains:\n- domain: vessel.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: vessel.land\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/security/vessel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Embedded Integrations
- GTM
- Integrations
- iPaaS
- Sales Engagement
- Unified API
---
