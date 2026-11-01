---
api_specs:
- filename: sitey-my-check-api-openapi.yml
  format: yaml
  label: sitey-my Check API
  slug: sitey-my-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitey-my/openapi/sitey-my-check-api-openapi.yml
- filename: sitey-my-domains-api-openapi.yml
  format: yaml
  label: sitey-my Domains API
  slug: sitey-my-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitey-my/openapi/sitey-my-domains-api-openapi.yml
- filename: sitey-my-subdomains-api-openapi.yml
  format: yaml
  label: sitey-my Subdomains API
  slug: sitey-my-subdomains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sitey-my/openapi/sitey-my-subdomains-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sitey.my
  spf: false
hosts:
- cert_expires: Jan 25 21:32:01 2027 GMT
  host: sitey.my
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sitey My Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sitey-my, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: sitey-my
provider_slug: sitey-my
slug: sitey-my-domain-security
source_filename: sitey-my-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sitey.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 21:32:01 2027 GMT\n  hsts: false\ndomains:\n- domain: sitey.my\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sitey-my/security/sitey-my-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- WebsiteBuilder
- NoSignUp
- Subdomain
- MCP
---
