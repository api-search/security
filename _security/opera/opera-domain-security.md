---
api_specs:
- filename: opera-ads-openapi.yml
  format: yaml
  label: Opera Ads Open API
  slug: opera-ads-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/openapi/opera-ads-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 iodef "mailto:hostmaster@opera.com"
  - 0 issue "sectigo.com"
  - 0 issue "trust-provider.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opera.com
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: opera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: ofa.adx.opera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Opera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opera, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Opera
provider_slug: opera
slug: opera-domain-security
source_filename: opera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\n- host: ofa.adx.opera.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opera.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 iodef \"mailto:hostmaster@opera.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"trust-provider.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/security/opera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Technology
- Advertising
- AdTech
- Browser
- Monetization
- OpenRTB
- Marketing
---
