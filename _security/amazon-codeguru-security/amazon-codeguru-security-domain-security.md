---
api_specs:
- filename: amazon-codeguru-security-accountconfiguration-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security AccountConfiguration API
  slug: amazon-codeguru-security-accountconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-accountconfiguration-api-openapi.yml
- filename: amazon-codeguru-security-batchgetfindings-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security BatchGetFindings API
  slug: amazon-codeguru-security-batchgetfindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-batchgetfindings-api-openapi.yml
- filename: amazon-codeguru-security-findings-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Findings API
  slug: amazon-codeguru-security-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-findings-api-openapi.yml
- filename: amazon-codeguru-security-metrics-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Metrics API
  slug: amazon-codeguru-security-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-metrics-api-openapi.yml
- filename: amazon-codeguru-security-scans-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Scans API
  slug: amazon-codeguru-security-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-scans-api-openapi.yml
- filename: amazon-codeguru-security-tags-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security Tags API
  slug: amazon-codeguru-security-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-tags-api-openapi.yml
- filename: amazon-codeguru-security-updateaccountconfiguration-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security UpdateAccountConfiguration API
  slug: amazon-codeguru-security-updateaccountconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-updateaccountconfiguration-api-openapi.yml
- filename: amazon-codeguru-security-uploadurl-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Security UploadUrl API
  slug: amazon-codeguru-security-uploadurl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/openapi/amazon-codeguru-security-uploadurl-api-openapi.yml
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
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: codeguru-security.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Codeguru Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon CodeGuru Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
slug: amazon-codeguru-security-domain-security
source_filename: amazon-codeguru-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: codeguru-security.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/security/amazon-codeguru-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
---
