---
api_specs:
- filename: exviv-com-discovery-api-openapi.yml
  format: yaml
  label: EXVIV Discovery API
  slug: exviv-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exviv-com/openapi/exviv-com-discovery-api-openapi.yml
- filename: exviv-com-paid-intel-api-openapi.yml
  format: yaml
  label: EXVIV Paid intel API
  slug: exviv-com-paid-intel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exviv-com/openapi/exviv-com-paid-intel-api-openapi.yml
- filename: exviv-com-paid-market-data-api-openapi.yml
  format: yaml
  label: EXVIV Paid market data API
  slug: exviv-com-paid-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exviv-com/openapi/exviv-com-paid-market-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: exviv.com
  spf: true
hosts:
- cert_expires: Dec 30 18:34:49 2026 GMT
  host: exviv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EXVIV Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EXVIV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EXVIV
provider_slug: exviv-com
slug: exviv-com-domain-security
source_filename: exviv-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exviv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 18:34:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: exviv.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/exviv-com/security/exviv-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Competitor Intelligence
- Market Research
- Software-as-a-Service
- Data Analytics
- Business Intelligence
---
