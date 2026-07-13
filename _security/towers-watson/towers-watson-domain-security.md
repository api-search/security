---
api_specs:
- filename: wtw-hr-portal-openapi.yml
  format: yaml
  label: WTW HR Portal
  slug: wtw-hr-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/towers-watson/refs/heads/main/openapi/wtw-hr-portal-openapi.yml
- filename: wtw-benefits-administration-openapi.yml
  format: yaml
  label: WTW Benefits Administration
  slug: wtw-benefits-administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/towers-watson/refs/heads/main/openapi/wtw-benefits-administration-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wtwco.com
  spf: true
hosts:
- cert_expires: Aug 25 06:40:43 2026 GMT
  host: www.wtwco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.wtwco.com
  https: false
kind: domain-security
layout: security
method: probed
name: Towers Watson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Towers Watson, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Towers Watson
provider_slug: towers-watson
slug: towers-watson-domain-security
source_filename: towers-watson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wtwco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 06:40:43 2026 GMT\n  hsts: null\n- host: api.wtwco.com\n  https: false\ndomains:\n- domain: wtwco.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/towers-watson/refs/heads/main/security/towers-watson-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Human Resources
- Risk Management
- Benefits
- Consulting
- Actuarial
- Insurance Brokerage
- Human Capital
---
