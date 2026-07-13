---
api_specs:
- filename: index
  format: yaml
  label: Acumatica REST API
  slug: acumatica-rest-api
  spec_type: OpenAPI
  url: https://your-instance.acumatica.com/swagger/ui/index
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acumatica.com
  spf: true
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: www.acumatica.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: your-instance.acumatica.com
  https: false
kind: domain-security
layout: security
method: probed
name: Acumatica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acumatica, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Acumatica
provider_slug: acumatica
slug: acumatica-domain-security
source_filename: acumatica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acumatica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: your-instance.acumatica.com\n  https: false\ndomains:\n- domain: acumatica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acumatica/refs/heads/main/security/acumatica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Cloud ERP
- Financial Management
- Inventory
- Manufacturing
- Distribution
- Project Accounting
- CRM
- Business Management
---
