---
api_specs:
- filename: connected2fiber-openapi-generated.yml
  format: yaml
  label: Connected2fiber API
  slug: connected2fiber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connected2fiber/refs/heads/main/openapi/_ae-authored/connected2fiber-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: connectbase.com
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: www.connectbase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connected2Fiber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connected2fiber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Connected2fiber
provider_slug: connected2fiber
slug: connected2fiber-domain-security
source_filename: connected2fiber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.connectbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: connectbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connected2fiber/refs/heads/main/security/connected2fiber-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Connectivity
- SaaS
- B2B
- Platform
- Network
---
