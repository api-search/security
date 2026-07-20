---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Klutch Public API
  slug: klutch-public-api
  spec_type: Postman
  url: https://api-docs.klutchcard.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: klutchcard.com
  spf: true
hosts:
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: klutchcard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:42:05 2026 GMT
  host: www.klutchcard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: graphql.klutchcard.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klutch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klutch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Klutch
provider_slug: klutch
slug: klutch-domain-security
source_filename: klutch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: klutchcard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.klutchcard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:42:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graphql.klutchcard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: klutchcard.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klutch/refs/heads/main/security/klutch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Fintech
- Credit Cards
- Payments
- Card Issuing
- Virtual Cards
- Transactions
- Spend Management
- Personal Finance
- GraphQL
- Embedded Finance
- Agents
---
