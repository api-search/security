---
api_specs:
- filename: steadily-account-api-openapi.yml
  format: yaml
  label: Steadily Account API
  slug: steadily-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-account-api-openapi.yml
- filename: steadily-draft-quote-api-openapi.yml
  format: yaml
  label: Steadily Draft Quote API
  slug: steadily-draft-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-draft-quote-api-openapi.yml
- filename: steadily-lead-referrals-api-openapi.yml
  format: yaml
  label: Steadily Lead Referrals API
  slug: steadily-lead-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-lead-referrals-api-openapi.yml
- filename: steadily-lender-api-openapi.yml
  format: yaml
  label: Steadily Lender API
  slug: steadily-lender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-lender-api-openapi.yml
- filename: steadily-policy-api-openapi.yml
  format: yaml
  label: Steadily Policy API
  slug: steadily-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-policy-api-openapi.yml
- filename: steadily-quote-estimates-api-openapi.yml
  format: yaml
  label: Steadily Quote Estimates API
  slug: steadily-quote-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-quote-estimates-api-openapi.yml
- filename: steadily-quote-offer-api-openapi.yml
  format: yaml
  label: Steadily Quote Offer API
  slug: steadily-quote-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-quote-offer-api-openapi.yml
- filename: steadily-reporting-api-openapi.yml
  format: yaml
  label: Steadily Reporting API
  slug: steadily-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-reporting-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: steadily.com
  spf: true
hosts:
- cert_expires: Oct  3 06:27:41 2026 GMT
  host: steadily.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Steadily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Steadily, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Steadily
provider_slug: steadily
slug: steadily-domain-security
source_filename: steadily-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: steadily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:27:41 2026 GMT\n  hsts: false\ndomains:\n- domain: steadily.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/security/steadily-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Insurance
- Landlord Insurance
- Insurtech
- Real-Estate
- Rental Property
---
