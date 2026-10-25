---
api_specs:
- filename: cello-events-api-openapi.yml
  format: yaml
  label: Cello Events API
  slug: cello-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-events-api-openapi.yml
- filename: cello-new-users-api-openapi.yml
  format: yaml
  label: Cello New Users API
  slug: cello-new-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-new-users-api-openapi.yml
- filename: cello-referral-codes-api-openapi.yml
  format: yaml
  label: Cello Referral Codes API
  slug: cello-referral-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-referral-codes-api-openapi.yml
- filename: cello-referrers-api-openapi.yml
  format: yaml
  label: Cello Referrers API
  slug: cello-referrers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-referrers-api-openapi.yml
- filename: cello-token-api-openapi.yml
  format: yaml
  label: Cello Token API
  slug: cello-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-token-api-openapi.yml
- filename: cello-events-v2-api-openapi.yml
  format: yaml
  label: Cello Events v2 API
  slug: cello-events-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-events-v2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cello.so
  spf: true
hosts:
- cert_expires: Nov 20 12:34:50 2026 GMT
  host: www.cello.so
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 09:42:43 2026 GMT
  host: docs.cello.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: api.cello.so
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cello Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cello, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cello
provider_slug: cello
slug: cello-domain-security
source_filename: cello-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cello.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 12:34:50 2026 GMT\n  hsts: false\n- host: docs.cello.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 09:42:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cello.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cello.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/security/cello-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Referral Marketing
- Affiliate Marketing
- Growth
- Software-as-a-Service
- Attribution
- Partner Programs
- Ai Enterprise Software
- A2A
---
