---
api_specs:
- filename: amcs-group-erp-openapi-original.json
  format: json
  label: AMCS Platform ERP REST API
  slug: amcs-platform-erp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-erp-openapi-original.json
- filename: amcs-group-core-openapi-original.json
  format: json
  label: AMCS Core API
  slug: amcs-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-core-openapi-original.json
- filename: amcs-group-pay-openapi-original.json
  format: json
  label: AMCS Pay External API
  slug: amcs-pay-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-pay-openapi-original.json
- filename: amcs-group-scale-openapi-original.json
  format: json
  label: AMCS Scale REST API
  slug: amcs-scale-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-scale-openapi-original.json
- filename: amcs-group-tlv-openapi-original.json
  format: json
  label: AMCS TLV External API
  slug: amcs-tlv-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-tlv-openapi-original.json
- filename: amcs-group-visionai-openapi-original.json
  format: json
  label: AMCS Vision AI External API
  slug: amcs-vision-ai-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-visionai-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amcsgroup.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: amcsplatform.com
  spf: false
hosts:
- cert_expires: Sep  3 23:43:39 2026 GMT
  host: www.amcsgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  9 14:01:22 2027 GMT
  host: ete-p5-tst-svc-core.amcsplatform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 31 14:18:42 2026 GMT
  host: eu1-pay-dev.amcsplatform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Amcs Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMCS Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AMCS Group
provider_slug: amcs-group
slug: amcs-group-domain-security
source_filename: amcs-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amcsgroup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  3 23:43:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ete-p5-tst-svc-core.amcsplatform.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  9 14:01:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eu1-pay-dev.amcsplatform.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 14:18:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amcsgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: amcsplatform.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/security/amcs-group-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Waste Management
- Recycling
- Transport
- Logistics
- Environmental
- ERP
- Payments
- Artificial Intelligence
- SaaS
---
