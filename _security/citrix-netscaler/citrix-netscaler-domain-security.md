---
api_specs:
- filename: citrix-netscaler-authentication-api-openapi.yml
  format: yaml
  label: Citrix NetScaler Authentication API
  slug: citrix-netscaler-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-authentication-api-openapi.yml
- filename: citrix-netscaler-cs-virtual-server-api-openapi.yml
  format: yaml
  label: Citrix NetScaler CS Virtual Server API
  slug: citrix-netscaler-cs-virtual-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-cs-virtual-server-api-openapi.yml
- filename: citrix-netscaler-lb-virtual-server-api-openapi.yml
  format: yaml
  label: Citrix NetScaler LB Virtual Server API
  slug: citrix-netscaler-lb-virtual-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-lb-virtual-server-api-openapi.yml
- filename: citrix-netscaler-ns-config-api-openapi.yml
  format: yaml
  label: Citrix NetScaler NS Config API
  slug: citrix-netscaler-ns-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-ns-config-api-openapi.yml
- filename: citrix-netscaler-statistics-api-openapi.yml
  format: yaml
  label: Citrix NetScaler Statistics API
  slug: citrix-netscaler-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-statistics-api-openapi.yml
- filename: citrix-netscaler-system-api-openapi.yml
  format: yaml
  label: Citrix NetScaler System API
  slug: citrix-netscaler-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netscaler.com
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.netscaler.com
  hsts: true
  hsts_max_age: 31449600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: developer-docs.netscaler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Citrix Netscaler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citrix NetScaler, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Citrix NetScaler
provider_slug: citrix-netscaler
slug: citrix-netscaler-domain-security
source_filename: citrix-netscaler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netscaler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31449600\n- host: developer-docs.netscaler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netscaler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/security/citrix-netscaler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Gateway
- Application Delivery Controller
- Application Security
- Load Balancing
- SSL Offloading
- Traffic Management
- Web Application Firewall
---
