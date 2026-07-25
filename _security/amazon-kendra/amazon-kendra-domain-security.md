---
api_specs:
- filename: amazon-kendra-data-sources-api-openapi.yml
  format: yaml
  label: Amazon Kendra Data Sources API
  slug: amazon-kendra-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-data-sources-api-openapi.yml
- filename: amazon-kendra-documents-api-openapi.yml
  format: yaml
  label: Amazon Kendra Documents API
  slug: amazon-kendra-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-documents-api-openapi.yml
- filename: amazon-kendra-experience-api-openapi.yml
  format: yaml
  label: Amazon Kendra Experience API
  slug: amazon-kendra-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-experience-api-openapi.yml
- filename: amazon-kendra-faqs-api-openapi.yml
  format: yaml
  label: Amazon Kendra FAQs API
  slug: amazon-kendra-faqs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-faqs-api-openapi.yml
- filename: amazon-kendra-indexes-api-openapi.yml
  format: yaml
  label: Amazon Kendra Indexes API
  slug: amazon-kendra-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-indexes-api-openapi.yml
- filename: amazon-kendra-queries-api-openapi.yml
  format: yaml
  label: Amazon Kendra Queries API
  slug: amazon-kendra-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-queries-api-openapi.yml
- filename: amazon-kendra-query-suggestions-api-openapi.yml
  format: yaml
  label: Amazon Kendra Query Suggestions API
  slug: amazon-kendra-query-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-query-suggestions-api-openapi.yml
- filename: amazon-kendra-thesaurus-api-openapi.yml
  format: yaml
  label: Amazon Kendra Thesaurus API
  slug: amazon-kendra-thesaurus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/openapi/amazon-kendra-thesaurus-api-openapi.yml
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
- host: kendra.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Kendra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Kendra, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Kendra
provider_slug: amazon-kendra
slug: amazon-kendra-domain-security
source_filename: amazon-kendra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: kendra.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/security/amazon-kendra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Enterprise Search
- Knowledge Management
- Machine Learning
- Natural Language
---
