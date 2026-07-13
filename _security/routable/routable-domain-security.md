---
api_specs:
- filename: routable-openapi.yml
  format: yaml
  label: Routable Vendors API
  slug: vendors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Payables API
  slug: payables
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Receivables API
  slug: receivables
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Funding Sources API
  slug: funding-sources
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
- filename: routable-openapi.yml
  format: yaml
  label: Routable Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/openapi/routable-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@routable.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: routable.com
  spf: true
hosts:
- cert_expires: Aug 25 06:03:01 2026 GMT
  host: www.routable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:29:25 2026 GMT
  host: developers.routable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.routable.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Routable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Routable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Routable
provider_slug: routable
slug: routable-domain-security
source_filename: routable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.routable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 06:03:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.routable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:29:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.routable.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: routable.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@routable.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routable/refs/heads/main/security/routable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Accounts Payable
- Accounts Receivable
- B2B Payments
- Mass Payouts
- FinTech
---
