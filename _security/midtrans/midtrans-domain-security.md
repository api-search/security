---
api_specs:
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Snap API
  slug: midtrans-snap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Core API
  slug: midtrans-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Card Tokenization API
  slug: midtrans-card-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans GoPay Tokenization API
  slug: midtrans-gopay-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Payment Link API
  slug: midtrans-payment-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Subscription API
  slug: midtrans-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Iris Disbursement API
  slug: midtrans-iris-disbursement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: midtrans.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:mailgun.org include:10122944f.ppspf.net include:2528720.spf02.hubspotemail.net ~all
- caa: []
  dnssec: false
  domain: api.midtrans.com
  notes: Resolves via CNAME to Alibaba Cloud WAF; no CAA record served at this name.
hosts:
- cert_expires: Aug 13 20:13:32 2026 GMT
  cert_issuer: Google Trust Services
  host: midtrans.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  cert_issuer: ZeroSSL
  host: api.midtrans.com
  hsts: unknown
  https: true
  notes: Fronted by Alibaba Cloud WAF (CNAME to *.aliyunwaf2.com); HEAD probe blocked, so the HSTS header could not be read.
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:29:11 2026 GMT
  cert_issuer: Google Trust Services
  host: docs.midtrans.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  cert_issuer: ZeroSSL
  host: app.midtrans.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Midtrans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Midtrans, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Midtrans
provider_slug: midtrans
slug: midtrans-domain-security
source_filename: midtrans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: midtrans.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 20:13:32 2026 GMT\n  cert_issuer: Google Trust Services\n  hsts: false\n- host: api.midtrans.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  cert_issuer: ZeroSSL\n  hsts: unknown\n  notes: Fronted by Alibaba Cloud WAF (CNAME to *.aliyunwaf2.com); HEAD probe blocked, so the HSTS header could not be read.\n- host: docs.midtrans.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:29:11 2026 GMT\n  cert_issuer: Google Trust Services\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.midtrans.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  cert_issuer: ZeroSSL\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: midtrans.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1\
  \ include:_spf.google.com include:mailgun.org include:10122944f.ppspf.net include:2528720.spf02.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: reject\n- domain: api.midtrans.com\n  dnssec: false\n  caa: []\n  notes: Resolves via CNAME to Alibaba Cloud WAF; no CAA record served at this name.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/security/midtrans-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Indonesia
- Southeast Asia
- Snap
- E-Wallet
- Virtual Account
- Cards
- Bank Transfer
- Fintech
---
