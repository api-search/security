---
api_specs:
- filename: payt-openapi-original.json
  format: json
  label: Payt Customer API v1
  slug: payt-customer-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payt/refs/heads/main/openapi/payt-openapi-original.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:devops@paytsoftware.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: paytsoftware.com
  spf: true
hosts:
- host: www.paytsoftware.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: api.paytsoftware.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: demo-api.paytsoftware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Payt
provider_slug: payt
slug: payt-domain-security
source_filename: payt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paytsoftware.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: api.paytsoftware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\n- host: demo-api.paytsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: paytsoftware.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:devops@paytsoftware.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payt/refs/heads/main/security/payt-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Applicative SaaS
- Accounts Receivable
- Order to Cash
- Invoicing
- Debt Collection
- Payments
- Fintech
- Credit Management
- Netherlands
---
