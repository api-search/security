---
api_specs:
- filename: amazon-codeguru-reviewer-associations-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Reviewer Associations API
  slug: amazon-codeguru-reviewer-associations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/openapi/amazon-codeguru-reviewer-associations-api-openapi.yml
- filename: amazon-codeguru-reviewer-codereviews-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Reviewer Codereviews API
  slug: amazon-codeguru-reviewer-codereviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/openapi/amazon-codeguru-reviewer-codereviews-api-openapi.yml
- filename: amazon-codeguru-reviewer-codereviews-type-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Reviewer Codereviews#Type API
  slug: amazon-codeguru-reviewer-codereviews-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/openapi/amazon-codeguru-reviewer-codereviews-type-api-openapi.yml
- filename: amazon-codeguru-reviewer-feedback-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Reviewer Feedback API
  slug: amazon-codeguru-reviewer-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/openapi/amazon-codeguru-reviewer-feedback-api-openapi.yml
- filename: amazon-codeguru-reviewer-tags-api-openapi.yml
  format: yaml
  label: Amazon CodeGuru Reviewer Tags API
  slug: amazon-codeguru-reviewer-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/openapi/amazon-codeguru-reviewer-tags-api-openapi.yml
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
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: codeguru-reviewer.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Codeguru Reviewer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon CodeGuru Reviewer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
slug: amazon-codeguru-reviewer-domain-security
source_filename: amazon-codeguru-reviewer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: codeguru-reviewer.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/security/amazon-codeguru-reviewer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon
- Code Review
- Security
- DevOps
- Machine-Learning
- Developer Tools
---
