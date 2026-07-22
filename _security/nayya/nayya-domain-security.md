---
api_specs:
- filename: nayya-accounts-openapi.json
  format: json
  label: Nayya Accounts API
  slug: nayya-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-accounts-openapi.json
- filename: nayya-benefits-openapi.json
  format: json
  label: Nayya Benefits API
  slug: nayya-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-benefits-openapi.json
- filename: nayya-choose-openapi.json
  format: json
  label: Nayya Choose API
  slug: nayya-choose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/openapi/nayya-choose-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nayya.com
  spf: true
hosts:
- cert_expires: Sep 21 15:23:32 2026 GMT
  host: nayya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nayya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nayya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nayya
provider_slug: nayya
slug: nayya-domain-security
source_filename: nayya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nayya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:23:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nayya.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nayya/refs/heads/main/security/nayya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employee Benefits
- Insurance
- Insurtech
- Health
- Decision Support
- HR Tech
- Enrollment
- Recommendations
- Artificial Intelligence
---
