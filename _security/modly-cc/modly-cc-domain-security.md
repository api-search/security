---
api_specs:
- filename: modly-cc-guild-api-openapi.yml
  format: yaml
  label: Modly Guild API
  slug: modly-cc-guild-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modly-cc/openapi/modly-cc-guild-api-openapi.yml
- filename: modly-cc-leveling-api-openapi.yml
  format: yaml
  label: Modly Leveling API
  slug: modly-cc-leveling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modly-cc/openapi/modly-cc-leveling-api-openapi.yml
- filename: modly-cc-moderation-api-openapi.yml
  format: yaml
  label: Modly Moderation API
  slug: modly-cc-moderation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modly-cc/openapi/modly-cc-moderation-api-openapi.yml
- filename: modly-cc-modules-api-openapi.yml
  format: yaml
  label: Modly Modules API
  slug: modly-cc-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modly-cc/openapi/modly-cc-modules-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: modly.cc
  spf: false
hosts:
- cert_expires: Jan  4 07:26:38 2027 GMT
  host: modly.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Modly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Modly
provider_slug: modly-cc
slug: modly-cc-domain-security
source_filename: modly-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modly.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 07:26:38 2027 GMT\n  hsts: false\ndomains:\n- domain: modly.cc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/modly-cc/security/modly-cc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Discord
- Bot
- Moderation
- Artificial Intelligence
- Community
---
