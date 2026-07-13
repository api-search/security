---
api_specs:
- filename: commercetools-http-api-openapi.yml
  format: yaml
  label: Commercetools HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-http-api-openapi.yml
- filename: commercetools-import-api-openapi.yml
  format: yaml
  label: Commercetools Import API
  slug: import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-import-api-openapi.yml
- filename: commercetools-change-history-api-openapi.yml
  format: yaml
  label: Commercetools Change History API
  slug: change-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-change-history-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "rapidssl.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commercetools.com
  spf: true
hosts:
- cert_expires: Sep 12 12:45:08 2026 GMT
  host: commercetools.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 10:16:07 2026 GMT
  host: docs.commercetools.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commercetools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for commercetools, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: commercetools
provider_slug: commercetools
slug: commercetools-domain-security
source_filename: commercetools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commercetools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 12:45:08 2026 GMT\n  hsts: false\n- host: docs.commercetools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 10:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: commercetools.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/security/commercetools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Composable Commerce
- E-Commerce
- GraphQL
- REST
- SDK
---
