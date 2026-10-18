---
api_specs:
- filename: openaire-broker-api-openapi.yml
  format: yaml
  label: OpenAIRE Broker API
  slug: openaire-broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openaire/refs/heads/main/openapi/openaire-broker-api-openapi.yml
- filename: openaire-oidc-api-openapi.yml
  format: yaml
  label: OpenAIRE Oidc API
  slug: openaire-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openaire/refs/heads/main/openapi/openaire-oidc-api-openapi.yml
- filename: openaire-openaire-api-api-openapi.yml
  format: yaml
  label: OpenAIRE OpenAIRE API
  slug: openaire-openaire-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openaire/refs/heads/main/openapi/openaire-openaire-api-api-openapi.yml
- filename: openaire-skg-if-api-openapi.yml
  format: yaml
  label: OpenAIRE Skg If API
  slug: openaire-skg-if-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openaire/refs/heads/main/openapi/openaire-skg-if-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openaire.eu
  spf: true
hosts:
- cert_expires: Nov 20 10:50:10 2026 GMT
  host: www.openaire.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openaire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAIRE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenAIRE
provider_slug: openaire
slug: openaire-domain-security
source_filename: openaire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openaire.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 10:50:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openaire.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openaire/refs/heads/main/security/openaire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Open Science
- Research Infrastructure
- Europe
- Services
---
