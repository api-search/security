---
api_specs:
- filename: supabase-management-api-openapi.yml
  format: yaml
  label: Supabase Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/openapi/supabase-management-api-openapi.yml
- filename: supabase-auth-api-openapi.yml
  format: yaml
  label: Supabase Auth API
  slug: auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/openapi/supabase-auth-api-openapi.yml
- filename: supabase-storage-api-openapi.yml
  format: yaml
  label: Supabase Storage API
  slug: storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/openapi/supabase-storage-api-openapi.yml
- filename: supabase-database-rest-api-openapi.yml
  format: yaml
  label: Supabase Database REST API
  slug: database-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/openapi/supabase-database-rest-api-openapi.yml
- filename: supabase-edge-functions-api-openapi.yml
  format: yaml
  label: Supabase Edge Functions API
  slug: edge-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/openapi/supabase-edge-functions-api-openapi.yml
- filename: supabase-realtime-api-asyncapi.yml
  format: yaml
  label: Supabase Realtime API
  slug: realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/asyncapi/supabase-realtime-api-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: supabase.com
  spf: true
hosts:
- cert_expires: Aug  9 14:02:11 2026 GMT
  host: supabase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 10:30:56 2026 GMT
  host: api.supabase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Supabase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Supabase, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Supabase
provider_slug: supabase
slug: supabase-domain-security
source_filename: supabase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: supabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 14:02:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.supabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:30:56 2026 GMT\n  hsts: null\ndomains:\n- domain: supabase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supabase/refs/heads/main/security/supabase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backend As A Service
- PostgreSQL
- Open Source
- Authentication
- Real Time
- Storage
- Edge Functions
- Database
---
