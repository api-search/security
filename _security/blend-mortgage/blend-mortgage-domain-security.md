---
api_specs:
- filename: blend-mortgage-borrowers-parties-api-openapi.yml
  format: yaml
  label: Blend Borrowers & Parties API
  slug: blend-mortgage-borrowers-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-borrowers-parties-api-openapi.yml
- filename: blend-mortgage-closings-esignature-api-openapi.yml
  format: yaml
  label: Blend Closings & eSignature API
  slug: blend-mortgage-closings-esignature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-closings-esignature-api-openapi.yml
- filename: blend-mortgage-consumer-lending-deposit-api-openapi.yml
  format: yaml
  label: Blend Consumer Lending & Deposit API
  slug: blend-mortgage-consumer-lending-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-consumer-lending-deposit-api-openapi.yml
- filename: blend-mortgage-documents-disclosures-api-openapi.yml
  format: yaml
  label: Blend Documents & Disclosures API
  slug: blend-mortgage-documents-disclosures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-documents-disclosures-api-openapi.yml
- filename: blend-mortgage-events-webhooks-api-openapi.yml
  format: yaml
  label: Blend Events & Webhooks API
  slug: blend-mortgage-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-events-webhooks-api-openapi.yml
- filename: blend-mortgage-follow-ups-api-openapi.yml
  format: yaml
  label: Blend Follow-ups API
  slug: blend-mortgage-follow-ups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-follow-ups-api-openapi.yml
- filename: blend-mortgage-home-lending-applications-api-openapi.yml
  format: yaml
  label: Blend Home Lending Applications API
  slug: blend-mortgage-home-lending-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-home-lending-applications-api-openapi.yml
- filename: blend-mortgage-lenders-assignments-api-openapi.yml
  format: yaml
  label: Blend Lenders & Assignments API
  slug: blend-mortgage-lenders-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-lenders-assignments-api-openapi.yml
- filename: blend-mortgage-products-pricing-api-openapi.yml
  format: yaml
  label: Blend Products & Pricing API
  slug: blend-mortgage-products-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-products-pricing-api-openapi.yml
- filename: blend-mortgage-reporting-api-openapi.yml
  format: yaml
  label: Blend Reporting API
  slug: blend-mortgage-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-reporting-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blend.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blendlabs.com
  spf: true
hosts:
- cert_expires: Jul 25 04:16:51 2026 GMT
  host: blend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  4 02:53:41 2026 GMT
  host: developers.blend.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: api.blendlabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blend Mortgage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blend, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blend
provider_slug: blend-mortgage
slug: blend-mortgage-domain-security
source_filename: blend-mortgage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blend.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 25 04:16:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.blend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:53:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.blendlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: blend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: blendlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/security/blend-mortgage-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Digital Lending
- Mortgage
- Consumer Lending
- Account Opening
- Fintech
- Loan Origination
- Banking
- Financial-Services
---
