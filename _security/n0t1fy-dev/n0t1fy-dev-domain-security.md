---
api_specs:
- filename: n0t1fy-dev-health-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Health API
  slug: n0t1fy-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-health-api-openapi.yml
- filename: n0t1fy-dev-keys-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Keys API
  slug: n0t1fy-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-keys-api-openapi.yml
- filename: n0t1fy-dev-messages-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Messages API
  slug: n0t1fy-dev-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-messages-api-openapi.yml
- filename: n0t1fy-dev-verifications-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Verifications API
  slug: n0t1fy-dev-verifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-verifications-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: n0t1fy.dev
  spf: true
hosts:
- cert_expires: Dec 31 08:20:48 2026 GMT
  host: n0t1fy.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: N0T1Fy Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for n0t1fy-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: n0t1fy-dev
provider_slug: n0t1fy-dev
slug: n0t1fy-dev-domain-security
source_filename: n0t1fy-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: n0t1fy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 08:20:48 2026 GMT\n  hsts: false\ndomains:\n- domain: n0t1fy.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/n0t1fy-dev/security/n0t1fy-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SMS
- Georgia
- Transactional
- Developer-First
---
