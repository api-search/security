---
api_specs:
- filename: weglot-openapi.yml
  format: yaml
  label: Weglot Translate API
  slug: weglot-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weglot/refs/heads/main/openapi/weglot-openapi.yml
- filename: weglot-openapi.yml
  format: yaml
  label: Weglot Languages API
  slug: weglot-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weglot/refs/heads/main/openapi/weglot-openapi.yml
- filename: weglot-openapi.yml
  format: yaml
  label: Weglot Status API
  slug: weglot-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weglot/refs/heads/main/openapi/weglot-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: weglot.com
  spf: true
hosts:
- cert_expires: Sep 18 12:57:53 2026 GMT
  host: www.weglot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 18:53:42 2026 GMT
  host: developers.weglot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 12:40:01 2026 GMT
  host: api.weglot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weglot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weglot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Weglot
provider_slug: weglot
slug: weglot-domain-security
source_filename: weglot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weglot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 12:57:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.weglot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 18:53:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.weglot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 12:40:01 2026 GMT\n  hsts: null\ndomains:\n- domain: weglot.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weglot/refs/heads/main/security/weglot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Translation
- Localization
- Internationalization
- Machine Translation
- Multilingual
---
