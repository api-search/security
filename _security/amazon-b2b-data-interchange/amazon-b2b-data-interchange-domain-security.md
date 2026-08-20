---
api_specs:
- filename: amazon-b2b-data-interchange-capabilities-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Capabilities API
  slug: amazon-b2b-data-interchange-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-capabilities-api-openapi.yml
- filename: amazon-b2b-data-interchange-partnerships-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Partnerships API
  slug: amazon-b2b-data-interchange-partnerships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-partnerships-api-openapi.yml
- filename: amazon-b2b-data-interchange-profiles-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Profiles API
  slug: amazon-b2b-data-interchange-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-profiles-api-openapi.yml
- filename: amazon-b2b-data-interchange-tags-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Tags API
  slug: amazon-b2b-data-interchange-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-tags-api-openapi.yml
- filename: amazon-b2b-data-interchange-testing-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Testing API
  slug: amazon-b2b-data-interchange-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-testing-api-openapi.yml
- filename: amazon-b2b-data-interchange-transformers-api-openapi.yml
  format: yaml
  label: Amazon B2B Data Interchange Transformers API
  slug: amazon-b2b-data-interchange-transformers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/openapi/amazon-b2b-data-interchange-transformers-api-openapi.yml
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
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: b2bi.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: b2bi.us-west-2.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon B2B Data Interchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon B2B Data Interchange, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon B2B Data Interchange
provider_slug: amazon-b2b-data-interchange
slug: amazon-b2b-data-interchange-domain-security
source_filename: amazon-b2b-data-interchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: b2bi.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\n- host: b2bi.us-west-2.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/security/amazon-b2b-data-interchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EDI
- B2B
- Data Interchange
- Supply Chain
- Healthcare
- Financial-Services
- Amazon Web Services
---
