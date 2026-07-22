---
api_specs:
- filename: uncapped-partners-openapi-original.json
  format: json
  label: Uncapped Partners API
  slug: uncapped-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncapped/refs/heads/main/openapi/uncapped-partners-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: weareuncapped.com
  spf: true
hosts:
- cert_expires: Aug 27 07:24:26 2026 GMT
  host: weareuncapped.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 08:06:16 2026 GMT
  host: developers.weareuncapped.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 08:06:16 2026 GMT
  host: portal.weareuncapped.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uncapped Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uncapped, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Uncapped
provider_slug: uncapped
slug: uncapped-domain-security
source_filename: uncapped-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weareuncapped.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 07:24:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.weareuncapped.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 08:06:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.weareuncapped.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 08:06:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: weareuncapped.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncapped/refs/heads/main/security/uncapped-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- Embedded Finance
- Revenue-Based Financing
- Working Capital
- eCommerce
---
