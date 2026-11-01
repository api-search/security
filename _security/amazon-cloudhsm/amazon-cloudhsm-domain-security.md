---
api_specs:
- filename: amazon-cloudhsm-hapg-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Hapg API
  slug: amazon-cloudhsm-hapg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-hapg-api-openapi.yml
- filename: amazon-cloudhsm-hsm-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Hsm API
  slug: amazon-cloudhsm-hsm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-hsm-api-openapi.yml
- filename: amazon-cloudhsm-luna-client-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Luna Client API
  slug: amazon-cloudhsm-luna-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-luna-client-api-openapi.yml
- filename: amazon-cloudhsm-operations-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Operations API
  slug: amazon-cloudhsm-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-operations-api-openapi.yml
- filename: amazon-cloudhsm-tag-api-openapi.yml
  format: yaml
  label: Amazon CloudHSM Cloudhsm Tag API
  slug: amazon-cloudhsm-tag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudhsm/openapi/amazon-cloudhsm-tag-api-openapi.yml
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
- host: cloudhsm.us-east-1.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Cloudhsm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon CloudHSM, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon CloudHSM
provider_slug: amazon-cloudhsm
slug: amazon-cloudhsm-domain-security
source_filename: amazon-cloudhsm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: cloudhsm.us-east-1.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-cloudhsm/security/amazon-cloudhsm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CloudHSM
- Security
- Cryptography
- HSM
- Compliance
---
