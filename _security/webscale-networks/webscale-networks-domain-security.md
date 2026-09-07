---
api_specs:
- filename: webscale-networks-webscale-apis-openapi.json
  format: json
  label: Webscale APIs
  slug: webscale-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscale-networks/refs/heads/main/openapi/webscale-networks-webscale-apis-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: webscale.com
  spf: true
hosts:
- cert_expires: Nov 20 19:37:49 2026 GMT
  host: www.webscale.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 19:37:32 2026 GMT
  host: control.webscale.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 19:37:32 2026 GMT
  host: api.webscale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Webscale Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webscale Networks, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Webscale Networks
provider_slug: webscale-networks
slug: webscale-networks-domain-security
source_filename: webscale-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.webscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 19:37:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: control.webscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 19:37:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.webscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 19:37:32 2026 GMT\n  hsts: null\ndomains:\n- domain: webscale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webscale-networks/refs/heads/main/security/webscale-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ecommerce
- Cloud Hosting
- Content Delivery Network
- Application Delivery
- Web Application Firewall
- Edge Computing
- Managed Hosting
- Infrastructure
- Magento
- Adobe Commerce
- Observability
---
