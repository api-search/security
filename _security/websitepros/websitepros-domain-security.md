---
api_specs:
- filename: websitepros-domains-api-openapi.yml
  format: yaml
  label: WebsitePros Domains API
  slug: websitepros-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/openapi/websitepros-domains-api-openapi.yml
- filename: websitepros-health-api-openapi.yml
  format: yaml
  label: WebsitePros Health API
  slug: websitepros-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/openapi/websitepros-health-api-openapi.yml
- filename: websitepros-sales-orders-api-openapi.yml
  format: yaml
  label: WebsitePros Sales Orders API
  slug: websitepros-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/openapi/websitepros-sales-orders-api-openapi.yml
- filename: websitepros-service-orders-api-openapi.yml
  format: yaml
  label: WebsitePros Service Orders API
  slug: websitepros-service-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/openapi/websitepros-service-orders-api-openapi.yml
- filename: websitepros-sso-api-openapi.yml
  format: yaml
  label: WebsitePros SSO API
  slug: websitepros-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/openapi/websitepros-sso-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: web.com
  spf: true
hosts:
- cert_expires: Sep 28 21:46:28 2026 GMT
  host: www.web.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 01:26:41 2026 GMT
  host: api-docs.intl.web.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.nts.web.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Websitepros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WebsitePros, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WebsitePros
provider_slug: websitepros
slug: websitepros-domain-security
source_filename: websitepros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.web.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:46:28 2026 GMT\n  hsts: null\n- host: api-docs.intl.web.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 01:26:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nts.web.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: web.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/security/websitepros-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Website Builder
- Web Hosting
- Domains
- Small Business
- Digital Marketing
- E-Commerce
- Reseller
- Sales Orders
- Provisioning
- Single Sign-On
- Azure API Management
---
