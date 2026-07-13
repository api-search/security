---
api_specs:
- filename: braintree-payments-openapi.yml
  format: yaml
  label: Braintree Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-payments-openapi.yml
- filename: braintree-webhooks-asyncapi.yml
  format: yaml
  label: Braintree Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/asyncapi/braintree-webhooks-asyncapi.yml
- filename: braintree-payments-openapi.yml
  format: yaml
  label: Braintree Vault API
  slug: vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-payments-openapi.yml
- filename: braintree-subscriptions-openapi.yml
  format: yaml
  label: Braintree Subscriptions API
  slug: subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-subscriptions-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "quovadisglobal.com"
  - 0 issue "visa.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: paypal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: braintreegateway.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: developer.paypal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.braintreegateway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: payments.braintree-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Braintree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for braintree, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: braintree
provider_slug: braintree
slug: braintree-domain-security
source_filename: braintree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.paypal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.braintreegateway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\n- host: payments.braintree-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: paypal.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issue \"visa.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: braintreegateway.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/security/braintree-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
