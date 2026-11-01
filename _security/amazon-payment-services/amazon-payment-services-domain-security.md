---
api_specs:
- filename: amazon-payment-services-openapi-generated.yml
  format: yaml
  label: Amazon Payment Services API
  slug: amazon-payment-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-payment-services/openapi/_ae-authored/amazon-payment-services-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: paymentservices.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amazon Payment Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Payment Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Payment Services
provider_slug: amazon-payment-services
slug: amazon-payment-services-domain-security
source_filename: amazon-payment-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paymentservices.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-payment-services/security/amazon-payment-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- FinTech
- API
- E-commerce
- PaymentsGateway
---
