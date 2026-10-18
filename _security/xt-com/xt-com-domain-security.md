---
api_specs:
- filename: xt-com-basic-error-controller-api-openapi.yml
  format: yaml
  label: XT.COM Basic Error Controller API
  slug: xt-com-basic-error-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-basic-error-controller-api-openapi.yml
- filename: xt-com-default-api-openapi.yml
  format: yaml
  label: XT.COM 合约信息 API
  slug: xt-com-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-default-api-openapi.yml
- filename: xt-com-listenkey-api-openapi.yml
  format: yaml
  label: XT.COM Listen Key API
  slug: xt-com-listenkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-listenkey-api-openapi.yml
- filename: xt-com-order-api-openapi.yml
  format: yaml
  label: XT.COM 合约聪明钱 Order API
  slug: xt-com-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-order-api-openapi.yml
- filename: xt-com-symbol-controller-api-openapi.yml
  format: yaml
  label: XT.COM Symbol Controller API
  slug: xt-com-symbol-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-symbol-controller-api-openapi.yml
- filename: xt-com-v2-api-openapi.yml
  format: yaml
  label: XT.COM 获取交易对配置信息(v2) API
  slug: xt-com-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-v2-api-openapi.yml
- filename: xt-com-v3-api-openapi.yml
  format: yaml
  label: XT.COM 获取交易对配置信息(v3) API
  slug: xt-com-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-v3-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xt.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: www.xt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: doc.xt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: fapi.xt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Xt Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XT.COM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: XT.COM
provider_slug: xt-com
slug: xt-com-domain-security
source_filename: xt-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\n- host: doc.xt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\n- host: fapi.xt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: xt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/security/xt-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Futures
- Market Data
- Blockchain
---
