---
api_specs:
- filename: getagentmd-com-openapi.json
  format: json
  label: AgentMD API
  slug: agentmd-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getagentmd-com/openapi/getagentmd-com-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: getagentmd.com
  spf: false
hosts:
- cert_expires: Feb  1 01:42:32 2027 GMT
  host: getagentmd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 01:42:32 2027 GMT
  host: www.getagentmd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: AgentMD Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentMD, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AgentMD
provider_slug: getagentmd-com
slug: getagentmd-com-domain-security
source_filename: getagentmd-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getagentmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 01:42:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.getagentmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 01:42:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getagentmd.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getagentmd-com/security/getagentmd-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Conversion
- Markdown
- Agents
---
