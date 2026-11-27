---
api_specs:
- filename: mermail-app-agent-api-openapi.yml
  format: yaml
  label: Mermail Agent API
  slug: mermail-app-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mermail-app/openapi/mermail-app-agent-api-openapi.yml
- filename: mermail-app-mermail-agent-marketplace-api-openapi.yml
  format: yaml
  label: Mermail Mermail Agent Marketplace API
  slug: mermail-app-mermail-agent-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mermail-app/openapi/mermail-app-mermail-agent-marketplace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mermail.app
  spf: true
hosts:
- cert_expires: Jan  2 12:12:02 2027 GMT
  host: mermail.app
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mermail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mermail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mermail
provider_slug: mermail-app
slug: mermail-app-domain-security
source_filename: mermail-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mermail.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 12:12:02 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: mermail.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mermail-app/security/mermail-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email
- Artificial Intelligence
- Wallets
- Automation
---
