---
api_specs:
- filename: dev
  format: yaml
  label: Densify Public Cloud API
  slug: public-cloud-api
  spec_type: Postman
  url: https://www.densify.com/dev
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: densify.com
  spf: true
hosts:
- cert_expires: Aug 18 16:42:02 2026 GMT
  host: www.densify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 16:42:02 2026 GMT
  host: portal.densify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 16:42:02 2026 GMT
  host: api.densify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Densify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Densify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Densify
provider_slug: densify
slug: densify-domain-security
source_filename: densify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.densify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 16:42:02 2026 GMT\n  hsts: false\n- host: portal.densify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 16:42:02 2026 GMT\n  hsts: false\n- host: api.densify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 16:42:02 2026 GMT\n  hsts: false\ndomains:\n- domain: densify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/security/densify-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud Cost
- Container Optimization
- FinOps
- Kubernetes
- Machine Learning
- Recommendations
- Right-Sizing
---
