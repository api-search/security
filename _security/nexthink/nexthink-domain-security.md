---
api_specs:
- filename: nexthink-nql-api-openapi.json
  format: json
  label: Nexthink NQL API
  slug: nexthink-nql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-nql-api-openapi.json
- filename: nexthink-remote-actions-api-openapi.json
  format: json
  label: Nexthink Remote Actions API
  slug: nexthink-remote-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-remote-actions-api-openapi.json
- filename: nexthink-workflows-openapi.json
  format: json
  label: Nexthink Workflows API
  slug: nexthink-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-workflows-openapi.json
- filename: nexthink-enrichment-api-openapi.json
  format: json
  label: Nexthink Enrichment API
  slug: nexthink-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-enrichment-api-openapi.json
- filename: nexthink-campaigns-api-openapi.json
  format: json
  label: Nexthink Campaigns API
  slug: nexthink-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-campaigns-api-openapi.json
- filename: nexthink-data-management-api-openapi.json
  format: json
  label: Nexthink Data Management API
  slug: nexthink-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-data-management-api-openapi.json
- filename: nexthink-spark-api-openapi.json
  format: json
  label: Nexthink Spark API
  slug: nexthink-spark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-spark-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nexthink.com
  spf: true
hosts:
- cert_expires: Sep 19 15:32:18 2026 GMT
  host: nexthink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexthink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexthink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nexthink
provider_slug: nexthink
slug: nexthink-domain-security
source_filename: nexthink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexthink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:32:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nexthink.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/security/nexthink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Business Applications
- Digital Employee Experience
- Endpoint Analytics
- IT Operations
- Automation
- Observability
- DEX
---
