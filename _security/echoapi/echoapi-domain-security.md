---
api_specs:
- filename: echoapi-openapi-generated.yml
  format: yaml
  label: EchoAPI API
  slug: echoapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echoapi/refs/heads/main/openapi/_ae-authored/echoapi-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: echoapi.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.echoapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Echoapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EchoAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EchoAPI
provider_slug: echoapi
slug: echoapi-domain-security
source_filename: echoapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.echoapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: echoapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echoapi/refs/heads/main/security/echoapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API Platform
- Integration
- Developer Tools
- AI-powered
- Documentation
---
