---
api_specs:
- filename: astroclaw-xyz-forecasts-api-openapi.yml
  format: yaml
  label: Astroclaw Forecasts API
  slug: astroclaw-xyz-forecasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astroclaw-xyz/openapi/astroclaw-xyz-forecasts-api-openapi.yml
- filename: astroclaw-xyz-sign-api-openapi.yml
  format: yaml
  label: Astroclaw Sign API
  slug: astroclaw-xyz-sign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astroclaw-xyz/openapi/astroclaw-xyz-sign-api-openapi.yml
- filename: astroclaw-xyz-signs-json-api-openapi.yml
  format: yaml
  label: Astroclaw Signs.json API
  slug: astroclaw-xyz-signs-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astroclaw-xyz/openapi/astroclaw-xyz-signs-json-api-openapi.yml
- filename: astroclaw-xyz-webhooks-api-openapi.yml
  format: yaml
  label: Astroclaw Webhooks API
  slug: astroclaw-xyz-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astroclaw-xyz/openapi/astroclaw-xyz-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: astroclaw.xyz
  spf: false
hosts:
- cert_expires: Jan  6 11:00:39 2027 GMT
  host: astroclaw.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Astroclaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astroclaw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Astroclaw
provider_slug: astroclaw-xyz
slug: astroclaw-xyz-domain-security
source_filename: astroclaw-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astroclaw.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 11:00:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: astroclaw.xyz\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/astroclaw-xyz/security/astroclaw-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Astrology
- Artificial Intelligence
- Agents
- Horoscopes
- Data
---
