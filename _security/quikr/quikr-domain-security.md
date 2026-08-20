---
api_specs:
- filename: quikr-app-api-openapi.yml
  format: yaml
  label: Quikr App API
  slug: quikr-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quikr/refs/heads/main/openapi/quikr-app-api-openapi.yml
- filename: quikr-platform-api-openapi.yml
  format: yaml
  label: Quikr Platform API
  slug: quikr-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quikr/refs/heads/main/openapi/quikr-platform-api-openapi.yml
- filename: quikr-public-api-openapi.yml
  format: yaml
  label: Quikr Public API
  slug: quikr-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quikr/refs/heads/main/openapi/quikr-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quikr.com
  spf: true
hosts:
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: quikr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quikr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quikr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quikr
provider_slug: quikr
slug: quikr-domain-security
source_filename: quikr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quikr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: quikr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quikr/refs/heads/main/security/quikr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Classifieds
- Marketplace
- Real-Estate
- Automotive
- Job
- E-Commerce
- India
- Developer Platform
---
