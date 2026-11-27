---
api_specs:
- filename: awesome-tools-agent-api-openapi.yml
  format: yaml
  label: Awesome Tools Agent API
  slug: awesome-tools-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awesome-tools/openapi/awesome-tools-agent-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: awesome.tools
  spf: true
hosts:
- cert_expires: Jan 19 15:43:52 2027 GMT
  host: awesome.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Awesome Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Awesome Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Awesome Tools
provider_slug: awesome-tools
slug: awesome-tools-domain-security
source_filename: awesome-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: awesome.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 15:43:52 2027 GMT\n  hsts: false\ndomains:\n- domain: awesome.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/awesome-tools/security/awesome-tools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software Directory
- AI Tools
- Software-as-a-Service
- Reviews
- OpenAPI
---
