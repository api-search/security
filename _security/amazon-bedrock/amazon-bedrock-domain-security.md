---
api_specs:
- filename: amazon-bedrock-converse-api-openapi.yml
  format: yaml
  label: Amazon Bedrock Converse API
  slug: amazon-bedrock-converse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/openapi/amazon-bedrock-converse-api-openapi.yml
- filename: amazon-bedrock-custom-models-api-openapi.yml
  format: yaml
  label: Amazon Bedrock Custom Models API
  slug: amazon-bedrock-custom-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/openapi/amazon-bedrock-custom-models-api-openapi.yml
- filename: amazon-bedrock-foundation-models-api-openapi.yml
  format: yaml
  label: Amazon Bedrock Foundation Models API
  slug: amazon-bedrock-foundation-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/openapi/amazon-bedrock-foundation-models-api-openapi.yml
- filename: amazon-bedrock-inference-api-openapi.yml
  format: yaml
  label: Amazon Bedrock Inference API
  slug: amazon-bedrock-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/openapi/amazon-bedrock-inference-api-openapi.yml
- filename: amazon-bedrock-model-customization-api-openapi.yml
  format: yaml
  label: Amazon Bedrock Model Customization API
  slug: amazon-bedrock-model-customization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/openapi/amazon-bedrock-model-customization-api-openapi.yml
- filename: amazon-bedrock-provisioned-throughput-api-openapi.yml
  format: yaml
  label: Amazon Bedrock Provisioned Throughput API
  slug: amazon-bedrock-provisioned-throughput-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/openapi/amazon-bedrock-provisioned-throughput-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: bedrock.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Bedrock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Bedrock, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Bedrock
provider_slug: amazon-bedrock
slug: amazon-bedrock-domain-security
source_filename: amazon-bedrock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: bedrock.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/security/amazon-bedrock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Foundation Models
- Generative AI
- LLM
- Machine-Learning
- RAG
- Agents
- Responsible AI
---
