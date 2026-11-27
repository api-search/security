---
api_specs:
- filename: notanats-com-agent-api-candidates-api-openapi.yml
  format: yaml
  label: notanATS Agent API — candidates API
  slug: notanats-com-agent-api-candidates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-agent-api-candidates-api-openapi.yml
- filename: notanats-com-agent-api-directory-api-openapi.yml
  format: yaml
  label: notanATS Agent API — directory API
  slug: notanats-com-agent-api-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-agent-api-directory-api-openapi.yml
- filename: notanats-com-agent-api-positions-api-openapi.yml
  format: yaml
  label: notanATS Agent API — positions API
  slug: notanats-com-agent-api-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-agent-api-positions-api-openapi.yml
- filename: notanats-com-agent-api-proposals-api-openapi.yml
  format: yaml
  label: notanATS Agent API — proposals API
  slug: notanats-com-agent-api-proposals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-agent-api-proposals-api-openapi.yml
- filename: notanats-com-credential-management-manager-session-api-openapi.yml
  format: yaml
  label: notanATS Credential management — manager session API
  slug: notanats-com-credential-management-manager-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-credential-management-manager-session-api-openapi.yml
- filename: notanats-com-legacy-api-v1-data-reads-api-openapi.yml
  format: yaml
  label: notanATS Legacy /api/v1 — data reads API
  slug: notanats-com-legacy-api-v1-data-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-legacy-api-v1-data-reads-api-openapi.yml
- filename: notanats-com-oauth-admin-review-api-openapi.yml
  format: yaml
  label: notanATS OAuth — admin review API
  slug: notanats-com-oauth-admin-review-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-oauth-admin-review-api-openapi.yml
- filename: notanats-com-oauth-discovery-api-openapi.yml
  format: yaml
  label: notanATS OAuth — discovery API
  slug: notanats-com-oauth-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-oauth-discovery-api-openapi.yml
- filename: notanats-com-oauth-flow-api-openapi.yml
  format: yaml
  label: notanATS OAuth — flow API
  slug: notanats-com-oauth-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-oauth-flow-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: notanats.com
  spf: true
hosts:
- cert_expires: Feb 13 11:34:56 2027 GMT
  host: notanats.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: notanATS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for notanATS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: notanATS
provider_slug: notanats-com
slug: notanats-com-domain-security
source_filename: notanats-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notanats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 11:34:56 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: notanats.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/notanats-com/security/notanats-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Screening
- Hiring
- Hiring Managers
- Agents
- AI Screening
---
