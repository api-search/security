---
api_specs:
- filename: mixmax-openapi.yml
  format: yaml
  label: Mixmax REST API
  slug: mixmax-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mixmax.com
  spf: true
hosts:
- cert_expires: Sep 28 19:08:31 2026 GMT
  host: www.mixmax.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mixmax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mixmax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mixmax
provider_slug: mixmax
slug: mixmax-domain-security
source_filename: mixmax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mixmax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:08:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mixmax.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/security/mixmax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Saas
- Sales Engagement
- Email
- Sales
- CRM
- Productivity
- Meetings
- Sequences
---
