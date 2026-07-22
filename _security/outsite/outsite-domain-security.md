---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: outsite.co
  spf: true
hosts:
- cert_expires: Oct  5 13:47:43 2026 GMT
  host: outsite.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outsite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outsite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Outsite
provider_slug: outsite
slug: outsite-domain-security
source_filename: outsite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outsite.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 13:47:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: outsite.co\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outsite/refs/heads/main/security/outsite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Coliving
- Coworking
- Remote Work
- Digital Nomads
- Travel
- Hospitality
- Membership
- Community
---
