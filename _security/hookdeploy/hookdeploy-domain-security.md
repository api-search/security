---
api_specs:
- filename: hookdeploy-openapi-generated.yml
  format: yaml
  label: HookDeploy API
  slug: hookdeploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeploy/refs/heads/main/openapi/_ae-authored/hookdeploy-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hookdeploy.dev
  spf: true
hosts:
- cert_expires: Dec 18 05:38:01 2026 GMT
  host: hookdeploy.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hookdeploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HookDeploy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HookDeploy
provider_slug: hookdeploy
slug: hookdeploy-domain-security
source_filename: hookdeploy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hookdeploy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 05:38:01 2026 GMT\n  hsts: false\ndomains:\n- domain: hookdeploy.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hookdeploy/refs/heads/main/security/hookdeploy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Webhooks
- PrivateInfrastructure
- Security
- Integration
- DeveloperTools
---
