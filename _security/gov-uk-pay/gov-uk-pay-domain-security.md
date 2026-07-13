---
api_specs:
- filename: publicapi_spec.json
  format: json
  label: GOV.UK Pay API
  slug: govuk-pay-api
  spec_type: OpenAPI
  url: https://github.com/alphagov/pay-publicapi/blob/master/openapi/publicapi_spec.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: service.gov.uk
  spf: true
hosts:
- cert_expires: Sep 16 21:28:19 2026 GMT
  host: docs.payments.service.gov.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: publicapi.payments.service.gov.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gov Uk Pay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GOV.UK Pay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GOV.UK Pay
provider_slug: gov-uk-pay
slug: gov-uk-pay-domain-security
source_filename: gov-uk-pay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.payments.service.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 21:28:19 2026 GMT\n  hsts: false\n- host: publicapi.payments.service.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: service.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gov-uk-pay/refs/heads/main/security/gov-uk-pay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Government
- UK
- Public Sector
- REST
- PCI DSS
- Refunds
- Recurring Payments
- Webhooks
---
