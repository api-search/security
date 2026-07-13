---
api_specs:
- filename: anodot-openapi.yml
  format: yaml
  label: Anodot Business Monitoring API
  slug: anodot-business-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/openapi/anodot-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anodot.com
  spf: true
hosts:
- cert_expires: Sep 14 07:42:38 2026 GMT
  host: www.anodot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: cloudcost.anodot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: docs.anodot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anodot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anodot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anodot
provider_slug: anodot
slug: anodot-domain-security
source_filename: anodot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anodot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:42:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloudcost.anodot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.anodot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: anodot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anodot/refs/heads/main/security/anodot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Anomaly Detection
- Business Monitoring
- Cloud Cost Management
- FinOps
- Machine Learning
- Observability
---
