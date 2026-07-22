---
api_specs:
- filename: sigma-ratings-openapi-original.json
  format: json
  label: Sigma360 API
  slug: sigma360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/openapi/sigma-ratings-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sigmaratings.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sigma360.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: sigmaratings.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: api.sigma360.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sigma Ratings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sigma360, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sigma360
provider_slug: sigma-ratings
slug: sigma-ratings-domain-security
source_filename: sigma-ratings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sigmaratings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\n- host: api.sigma360.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sigmaratings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sigma360.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/security/sigma-ratings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Compliance
- Financial Crime
- KYC
- AML
- Sanctions Screening
- Risk Intelligence
- RegTech
- Adverse Media
---
