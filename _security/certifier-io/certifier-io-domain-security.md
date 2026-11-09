---
api_specs:
- filename: certifier-io-credential-interactions-api-openapi.yml
  format: yaml
  label: Certifier Credential Interactions API
  slug: certifier-io-credential-interactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certifier-io/openapi/certifier-io-credential-interactions-api-openapi.yml
- filename: certifier-io-credential-templates-api-openapi.yml
  format: yaml
  label: Certifier Credential Templates API
  slug: certifier-io-credential-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certifier-io/openapi/certifier-io-credential-templates-api-openapi.yml
- filename: certifier-io-credentials-api-openapi.yml
  format: yaml
  label: Certifier Credentials API
  slug: certifier-io-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certifier-io/openapi/certifier-io-credentials-api-openapi.yml
- filename: certifier-io-design-templates-api-openapi.yml
  format: yaml
  label: Certifier Design Templates API
  slug: certifier-io-design-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certifier-io/openapi/certifier-io-design-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: certifier.io
  spf: true
hosts:
- cert_expires: Dec 30 07:06:42 2026 GMT
  host: certifier.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Certifier Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certifier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Certifier
provider_slug: certifier-io
slug: certifier-io-domain-security
source_filename: certifier-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: certifier.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 07:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: certifier.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/certifier-io/security/certifier-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Certificate
- Artificial Intelligence
- Automation
- Credentials
---
