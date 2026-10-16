---
api_specs:
- filename: brokergenius-openapi-generated.yml
  format: yaml
  label: Brokergenius API
  slug: brokergenius-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brokergenius/refs/heads/main/openapi/_ae-authored/brokergenius-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brokergenius.ai
  spf: true
hosts:
- cert_expires: Dec 30 00:59:52 2026 GMT
  host: brokergenius.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brokergenius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brokergenius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brokergenius
provider_slug: brokergenius
slug: brokergenius-domain-security
source_filename: brokergenius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brokergenius.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 00:59:52 2026 GMT\n  hsts: false\ndomains:\n- domain: brokergenius.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brokergenius/refs/heads/main/security/brokergenius-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Customs
- AI
- Automation
- Brokerage
- Logistics
---
