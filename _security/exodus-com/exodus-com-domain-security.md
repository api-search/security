---
api_specs:
- filename: exodus-com-checkouts-api-openapi.yml
  format: yaml
  label: Exodus Checkouts API
  slug: exodus-com-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-checkouts-api-openapi.yml
- filename: exodus-com-payments-api-openapi.yml
  format: yaml
  label: Exodus Payments API
  slug: exodus-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-payments-api-openapi.yml
- filename: exodus-com-reports-api-openapi.yml
  format: yaml
  label: Exodus Reports API
  slug: exodus-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-reports-api-openapi.yml
- filename: exodus-com-settings-api-openapi.yml
  format: yaml
  label: Exodus Settings API
  slug: exodus-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-settings-api-openapi.yml
- filename: exodus-com-subscription-checkouts-api-openapi.yml
  format: yaml
  label: Exodus Subscription checkouts API
  slug: exodus-com-subscription-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-subscription-checkouts-api-openapi.yml
- filename: exodus-com-subscriptions-api-openapi.yml
  format: yaml
  label: Exodus Subscriptions API
  slug: exodus-com-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-subscriptions-api-openapi.yml
- filename: exodus-com-webhook-events-api-openapi.yml
  format: yaml
  label: Exodus Webhook events API
  slug: exodus-com-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-webhook-events-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops@exodus.io"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: exodus.com
  spf: true
hosts:
- cert_expires: Feb  9 19:57:31 2027 GMT
  host: exodus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Exodus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exodus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Exodus
provider_slug: exodus-com
slug: exodus-com-domain-security
source_filename: exodus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exodus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 19:57:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: exodus.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@exodus.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/exodus-com/security/exodus-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Wallets
- Finance
- Payments
- Security
---
