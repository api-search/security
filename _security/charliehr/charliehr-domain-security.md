---
api_specs:
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Team Members
  slug: team-members
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Leave / Absences
  slug: leave-absences
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Leave Allowances
  slug: leave-allowances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Company
  slug: company
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: charliehr.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.charliehr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: charliehr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charliehr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CharlieHR, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CharlieHR
provider_slug: charliehr
slug: charliehr-domain-security
source_filename: charliehr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.charliehr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: charliehr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: charliehr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/security/charliehr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- HR
- HRIS
- People
- Leave
- Time Off
---
