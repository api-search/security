---
api_specs:
- filename: billionverify-com-account-api-openapi.yml
  format: yaml
  label: BillionVerify Account API
  slug: billionverify-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-account-api-openapi.yml
- filename: billionverify-com-file-processing-api-openapi.yml
  format: yaml
  label: BillionVerify File Processing API
  slug: billionverify-com-file-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-file-processing-api-openapi.yml
- filename: billionverify-com-health-api-openapi.yml
  format: yaml
  label: BillionVerify Health API
  slug: billionverify-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-health-api-openapi.yml
- filename: billionverify-com-verification-api-openapi.yml
  format: yaml
  label: BillionVerify Verification API
  slug: billionverify-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-verification-api-openapi.yml
- filename: billionverify-com-webhooks-api-openapi.yml
  format: yaml
  label: BillionVerify Webhooks API
  slug: billionverify-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: billionverify.com
  spf: true
hosts:
- cert_expires: Dec 11 11:48:00 2026 GMT
  host: billionverify.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BillionVerify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BillionVerify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: BillionVerify
provider_slug: billionverify-com
slug: billionverify-com-domain-security
source_filename: billionverify-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billionverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 11:48:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: billionverify.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/billionverify-com/security/billionverify-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Verification
- Software-as-a-Service
- Data Quality
- B2B
---
