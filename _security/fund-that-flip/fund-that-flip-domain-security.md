---
api_specs:
- filename: fund-that-flip-flipperforce-public-api.yml
  format: yaml
  label: FlipperForce Public API
  slug: flipperforce-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-flipperforce-public-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: upright.us
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flipperforce.com
  spf: true
hosts:
- cert_expires: Oct 31 12:55:40 2026 GMT
  host: www.upright.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 10:11:14 2026 GMT
  host: www.flipperforce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:27:53 2026 GMT
  host: tools.flipperforce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fund That Flip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fund That Flip, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fund That Flip
provider_slug: fund-that-flip
slug: fund-that-flip-domain-security
source_filename: fund-that-flip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upright.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 12:55:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.flipperforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:11:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tools.flipperforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:27:53 2026 GMT\n  hsts: false\ndomains:\n- domain: upright.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: flipperforce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/security/fund-that-flip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Lending
- Construction
- Project Management
- Financial Services
- Investing
- Fintech
- Property Technology
- Accounting
---
