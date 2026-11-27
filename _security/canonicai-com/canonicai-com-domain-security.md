---
api_specs:
- filename: canonicai-com-answers-api-openapi.yml
  format: yaml
  label: CanonicAI Answers API
  slug: canonicai-com-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canonicai-com/openapi/canonicai-com-answers-api-openapi.yml
- filename: canonicai-com-canons-api-openapi.yml
  format: yaml
  label: CanonicAI Canons API
  slug: canonicai-com-canons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canonicai-com/openapi/canonicai-com-canons-api-openapi.yml
- filename: canonicai-com-llms-txt-api-openapi.yml
  format: yaml
  label: CanonicAI Llms.txt API
  slug: canonicai-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canonicai-com/openapi/canonicai-com-llms-txt-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: canonicai.com
  spf: false
hosts:
- cert_expires: Jan  8 21:05:24 2027 GMT
  host: canonicai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CanonicAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CanonicAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: CanonicAI
provider_slug: canonicai-com
slug: canonicai-com-domain-security
source_filename: canonicai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canonicai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 21:05:24 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: canonicai.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/canonicai-com/security/canonicai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Data Extraction
- Tagging
- CanonicalDatasets
- Automation
---
