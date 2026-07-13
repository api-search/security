---
api_specs:
- filename: hello-retail-openapi.yml
  format: yaml
  label: Hello Retail API
  slug: hello-retail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hello-retail/refs/heads/main/openapi/hello-retail-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: helloretail.com
  spf: true
hosts:
- cert_expires: Sep 28 02:59:49 2026 GMT
  host: developer.helloretail.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 06:03:45 2026 GMT
  host: www.helloretail.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: core.helloretail.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hello Retail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hello Retail, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hello Retail
provider_slug: hello-retail
slug: hello-retail-domain-security
source_filename: hello-retail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.helloretail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:59:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: www.helloretail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: core.helloretail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: helloretail.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hello-retail/refs/heads/main/security/hello-retail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- E-Commerce
- Personalization
- Product Recommendations
- Retail
---
