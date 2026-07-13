---
api_specs:
- filename: openapi.json
  format: json
  label: Einstein Vision API
  slug: einstein-vision-api
  spec_type: OpenAPI
  url: https://api.einstein.ai/v2/vision/openapi.json
- filename: openapi.json
  format: json
  label: Einstein Language API
  slug: einstein-language-api
  spec_type: OpenAPI
  url: https://api.einstein.ai/v2/language/openapi.json
- filename: salesforce-einstein-prediction-builder-openapi.yml
  format: yaml
  label: Einstein Prediction Builder API
  slug: einstein-prediction-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-prediction-builder-openapi.yml
- filename: salesforce-einstein-discovery-openapi.yml
  format: yaml
  label: Einstein Discovery API
  slug: einstein-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-discovery-openapi.yml
- filename: salesforce-einstein-bots-openapi.yml
  format: yaml
  label: Einstein Bots API
  slug: einstein-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-bots-openapi.yml
- filename: salesforce-einstein-gpt-openapi.yml
  format: yaml
  label: Einstein GPT API
  slug: einstein-gpt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-gpt-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salesforce.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: einstein.ai
  spf: false
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: developer.salesforce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.salesforce.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.einstein.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salesforce Einstein Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Einstein, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Einstein
provider_slug: salesforce-einstein
slug: salesforce-einstein-domain-security
source_filename: salesforce-einstein-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: www.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.einstein.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: einstein.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/security/salesforce-einstein-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Computer Vision
- CRM
- Machine Learning
- Natural Language Processing
- Predictive Analytics
- Salesforce
---
