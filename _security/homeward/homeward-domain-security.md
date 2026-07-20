---
api_specs:
- filename: homeward-offer-estimate-openapi.yml
  format: yaml
  label: Homeward Offer Estimate API
  slug: homeward-offer-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/homeward/refs/heads/main/openapi/homeward-offer-estimate-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: homeward.com
  spf: true
hosts:
- cert_expires: Sep 21 14:41:09 2026 GMT
  host: homeward.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.homeward.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Homeward Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homeward, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Homeward
provider_slug: homeward
slug: homeward-domain-security
source_filename: homeward-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homeward.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:41:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.homeward.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: homeward.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homeward/refs/heads/main/security/homeward-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Home Finance
- Mortgage
- Proptech
- Cash Offer
- Title
- Lending
---
