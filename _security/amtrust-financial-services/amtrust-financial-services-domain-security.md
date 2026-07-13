---
api_specs:
- filename: amtrust-financial-services-commercial-lines-api.yaml
  format: yaml
  label: AmTrust Commercial Lines API
  slug: commercial-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-commercial-lines-api.yaml
description: ''
domains:
- caa:
  - ves-io-235f76b6-e673-4a73-aa89-7927b57b12ad.ac.vh.ves.io.
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amtrustfinancial.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amtrustservices.com
  spf: true
hosts:
- cert_expires: Aug 18 14:53:38 2026 GMT
  host: amtrustfinancial.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.amtrustservices.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amtrust Financial Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AmTrust Financial Services, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
slug: amtrust-financial-services-domain-security
source_filename: amtrust-financial-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amtrustfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 14:53:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.amtrustservices.com\n  https: false\ndomains:\n- domain: amtrustfinancial.com\n  dnssec: false\n  caa:\n  - ves-io-235f76b6-e673-4a73-aa89-7927b57b12ad.ac.vh.ves.io.\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: amtrustservices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/security/amtrust-financial-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commercial Insurance
- Insurance
- Property And Casualty
- Small Business
- Workers Compensation
- Fortune 1000
---
