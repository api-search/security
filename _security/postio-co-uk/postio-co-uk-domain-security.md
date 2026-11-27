---
api_specs:
- filename: postio-co-uk-address-api-openapi.yml
  format: yaml
  label: Postio Address API
  slug: postio-co-uk-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postio-co-uk/openapi/postio-co-uk-address-api-openapi.yml
- filename: postio-co-uk-email-api-openapi.yml
  format: yaml
  label: Postio Email API
  slug: postio-co-uk-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postio-co-uk/openapi/postio-co-uk-email-api-openapi.yml
- filename: postio-co-uk-other-api-openapi.yml
  format: yaml
  label: Postio Other API
  slug: postio-co-uk-other-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postio-co-uk/openapi/postio-co-uk-other-api-openapi.yml
- filename: postio-co-uk-phone-api-openapi.yml
  format: yaml
  label: Postio Phone API
  slug: postio-co-uk-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postio-co-uk/openapi/postio-co-uk-phone-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: postio.co.uk
  spf: true
hosts:
- cert_expires: Jan 11 22:29:48 2027 GMT
  host: postio.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Postio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Postio
provider_slug: postio-co-uk
slug: postio-co-uk-domain-security
source_filename: postio-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postio.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 22:29:48 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: postio.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/postio-co-uk/security/postio-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- United Kingdom
- Address
- Email
- Phone
- Validation
---
