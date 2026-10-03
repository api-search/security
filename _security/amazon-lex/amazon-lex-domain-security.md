---
api_specs:
- filename: amazon-lex-bots-api-openapi.yml
  format: yaml
  label: Amazon Lex Bots API
  slug: amazon-lex-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-bots-api-openapi.yml
- filename: amazon-lex-builtins-api-openapi.yml
  format: yaml
  label: Amazon Lex Builtins API
  slug: amazon-lex-builtins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-builtins-api-openapi.yml
- filename: amazon-lex-createuploadurl-api-openapi.yml
  format: yaml
  label: Amazon Lex Createuploadurl API
  slug: amazon-lex-createuploadurl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-createuploadurl-api-openapi.yml
- filename: amazon-lex-exports-api-openapi.yml
  format: yaml
  label: Amazon Lex Exports API
  slug: amazon-lex-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-exports-api-openapi.yml
- filename: amazon-lex-imports-api-openapi.yml
  format: yaml
  label: Amazon Lex Imports API
  slug: amazon-lex-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-imports-api-openapi.yml
- filename: amazon-lex-policy-api-openapi.yml
  format: yaml
  label: Amazon Lex Policy API
  slug: amazon-lex-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-policy-api-openapi.yml
- filename: amazon-lex-tags-api-openapi.yml
  format: yaml
  label: Amazon Lex Tags API
  slug: amazon-lex-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-tags-api-openapi.yml
- filename: amazon-lex-testexecutions-api-openapi.yml
  format: yaml
  label: Amazon Lex Testexecutions API
  slug: amazon-lex-testexecutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-testexecutions-api-openapi.yml
- filename: amazon-lex-testsetdiscrepancy-api-openapi.yml
  format: yaml
  label: Amazon Lex Testsetdiscrepancy API
  slug: amazon-lex-testsetdiscrepancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-testsetdiscrepancy-api-openapi.yml
- filename: amazon-lex-testsetgenerations-api-openapi.yml
  format: yaml
  label: Amazon Lex Testsetgenerations API
  slug: amazon-lex-testsetgenerations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-testsetgenerations-api-openapi.yml
- filename: amazon-lex-testsets-api-openapi.yml
  format: yaml
  label: Amazon Lex Testsets API
  slug: amazon-lex-testsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/openapi/amazon-lex-testsets-api-openapi.yml
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
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: models-v2-lex.amazonaws.com
  https: false
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: models-v2-lex.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Amazon Lex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Lex, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Lex
provider_slug: amazon-lex
slug: amazon-lex-domain-security
source_filename: amazon-lex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: models-v2-lex.amazonaws.com\n  https: false\n- host: models-v2-lex.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/security/amazon-lex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Conversational AI
- Chatbots
- Natural Language Processing
- Speech
- Voice
- Contact Center
- Customer Service
---
