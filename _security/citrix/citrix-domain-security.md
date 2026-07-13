---
api_specs:
- filename: openapi
  format: yaml
  label: Citrix Virtual Apps and Desktops REST API
  slug: citrix-virtual-apps-and-desktops-rest-api
  spec_type: OpenAPI
  url: https://developer.citrix.com/citrix-virtual-apps-and-desktops/citrix-cvad-rest-apis/docs/openapi
- filename: citrix-adc-nitro-openapi.yml
  format: yaml
  label: Citrix ADC (NetScaler) NITRO API
  slug: citrix-adc-netscaler-nitro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/openapi/citrix-adc-nitro-openapi.yml
- filename: openapi
  format: yaml
  label: Citrix DaaS REST API
  slug: citrix-daas-rest-api
  spec_type: OpenAPI
  url: https://developer.citrix.com/citrix-daas/citrix-daas-rest-apis/docs/openapi
- filename: citrix-cloud-openapi.yml
  format: yaml
  label: Citrix Cloud API
  slug: citrix-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/openapi/citrix-cloud-openapi.yml
- filename: citrix-storefront-web-openapi.yml
  format: yaml
  label: Citrix StoreFront Web API
  slug: citrix-storefront-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/openapi/citrix-storefront-web-openapi.yml
- filename: citrix-endpoint-management-openapi.yml
  format: yaml
  label: Citrix Endpoint Management REST API
  slug: citrix-endpoint-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/openapi/citrix-endpoint-management-openapi.yml
- filename: citrix-secure-private-access-openapi.yml
  format: yaml
  label: Citrix Secure Private Access API
  slug: citrix-secure-private-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/openapi/citrix-secure-private-access-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: citrix.com
  spf: true
hosts:
- cert_expires: Aug 11 23:59:59 2026 GMT
  host: developer-docs.citrix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.citrix.com
  hsts: true
  hsts_max_age: 31449600
  https: true
  tls_version: TLSv1.3
- host: developer.citrix.com
  https: false
kind: domain-security
layout: security
method: probed
name: Citrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citrix, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Citrix
provider_slug: citrix
slug: citrix-domain-security
source_filename: citrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer-docs.citrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.citrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31449600\n- host: developer.citrix.com\n  https: false\ndomains:\n- domain: citrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/security/citrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Delivery
- Desktop-As-A-Service
- Networking
- Virtualization
- Workspace
- Fortune 1000
---
