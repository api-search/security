---
api_specs:
- filename: usebraintrust-network-stats-openapi.yml
  format: yaml
  label: Braintrust Network Stats API
  slug: braintrust-network-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usebraintrust/refs/heads/main/openapi/usebraintrust-network-stats-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: usebraintrust.com
  spf: true
hosts:
- cert_expires: Aug 30 03:54:11 2026 GMT
  host: www.usebraintrust.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usebraintrust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Braintrust (Talent Network), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Braintrust (Talent Network)
provider_slug: usebraintrust
slug: usebraintrust-domain-security
source_filename: usebraintrust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usebraintrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:54:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usebraintrust.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usebraintrust/refs/heads/main/security/usebraintrust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Talent Marketplace
- AI Recruiting
- Hiring
- Freelancing
- Workforce Automation
- BTRST Token
- Web3
---
