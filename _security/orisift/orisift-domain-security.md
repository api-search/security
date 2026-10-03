---
api_specs:
- filename: orisift-lookup-api-openapi.yml
  format: yaml
  label: Orisift Lookup API
  slug: orisift-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orisift/refs/heads/main/openapi/orisift-lookup-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orisift.com
  spf: true
hosts:
- cert_expires: Dec 22 12:02:17 2026 GMT
  host: orisift.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orisift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orisift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Orisift
provider_slug: orisift
slug: orisift-domain-security
source_filename: orisift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orisift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 12:02:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orisift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orisift/refs/heads/main/security/orisift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Validation
- Phone
- Email
- IP
- Domain
---
