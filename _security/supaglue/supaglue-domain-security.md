---
api_specs:
- filename: supaglue-management-api-openapi.yml
  format: yaml
  label: Supaglue Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supaglue/refs/heads/main/openapi/supaglue-management-api-openapi.yml
- filename: supaglue-crm-api-openapi.yml
  format: yaml
  label: Supaglue Unified CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supaglue/refs/heads/main/openapi/supaglue-crm-api-openapi.yml
- filename: supaglue-engagement-api-openapi.yml
  format: yaml
  label: Supaglue Unified Engagement API
  slug: engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supaglue/refs/heads/main/openapi/supaglue-engagement-api-openapi.yml
- filename: supaglue-ticketing-api-openapi.yml
  format: yaml
  label: Supaglue Unified Ticketing API
  slug: ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supaglue/refs/heads/main/openapi/supaglue-ticketing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: supaglue.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: supaglue.io
  spf: false
hosts:
- host: www.supaglue.com
  https: false
- cert_expires: Sep 15 16:21:21 2026 GMT
  host: docs.supaglue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.supaglue.io
  https: false
kind: domain-security
layout: security
method: probed
name: Supaglue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Supaglue, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Supaglue
provider_slug: supaglue
slug: supaglue-domain-security
source_filename: supaglue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.supaglue.com\n  https: false\n- host: docs.supaglue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:21:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.supaglue.io\n  https: false\ndomains:\n- domain: supaglue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: supaglue.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supaglue/refs/heads/main/security/supaglue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- HRIS
- Unified API
- Open Source
- Integrations
- Sales Engagement
---
