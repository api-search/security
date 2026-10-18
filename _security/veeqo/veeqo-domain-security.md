---
api_specs:
- filename: veeqo-current-user-api-openapi.yml
  format: yaml
  label: Veeqo Current User API
  slug: veeqo-current-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeqo/refs/heads/main/openapi/veeqo-current-user-api-openapi.yml
- filename: veeqo-oauth-api-openapi.yml
  format: yaml
  label: Veeqo OAuth API
  slug: veeqo-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeqo/refs/heads/main/openapi/veeqo-oauth-api-openapi.yml
- filename: veeqo-orders-api-openapi.yml
  format: yaml
  label: Veeqo Orders API
  slug: veeqo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeqo/refs/heads/main/openapi/veeqo-orders-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: veeqo.com
  spf: true
hosts:
- cert_expires: Apr 15 07:21:34 2027 GMT
  host: www.veeqo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Veeqo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veeqo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Veeqo
provider_slug: veeqo
slug: veeqo-domain-security
source_filename: veeqo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veeqo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 15 07:21:34 2027 GMT\n  hsts: false\ndomains:\n- domain: veeqo.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veeqo/refs/heads/main/security/veeqo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Inventory
- order-fulfillment
- multi-channel
- Software-as-a-Service
---
