---
api_specs:
- filename: findymail-contacts-api-openapi.yml
  format: yaml
  label: Findymail Contacts API
  slug: findymail-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-contacts-api-openapi.yml
- filename: findymail-email-finder-api-openapi.yml
  format: yaml
  label: Findymail Email Finder API
  slug: findymail-email-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-email-finder-api-openapi.yml
- filename: findymail-email-verifier-api-openapi.yml
  format: yaml
  label: Findymail Email Verifier API
  slug: findymail-email-verifier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-email-verifier-api-openapi.yml
- filename: findymail-exclusion-lists-api-openapi.yml
  format: yaml
  label: Findymail Exclusion Lists API
  slug: findymail-exclusion-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-exclusion-lists-api-openapi.yml
- filename: findymail-intellimatch-api-openapi.yml
  format: yaml
  label: Findymail Intellimatch API
  slug: findymail-intellimatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-intellimatch-api-openapi.yml
- filename: findymail-misc-api-openapi.yml
  format: yaml
  label: Findymail Misc API
  slug: findymail-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-misc-api-openapi.yml
- filename: findymail-phone-finder-api-openapi.yml
  format: yaml
  label: Findymail Phone Finder API
  slug: findymail-phone-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-phone-finder-api-openapi.yml
- filename: findymail-signals-api-openapi.yml
  format: yaml
  label: Findymail Signals API
  slug: findymail-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-signals-api-openapi.yml
- filename: findymail-technologies-api-openapi.yml
  format: yaml
  label: Findymail Technologies API
  slug: findymail-technologies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-technologies-api-openapi.yml
- filename: findymail-usage-api-openapi.yml
  format: yaml
  label: Findymail Usage API
  slug: findymail-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: findymail.com
  spf: true
hosts:
- cert_expires: Jan 19 17:48:07 2027 GMT
  host: findymail.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Findymail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Findymail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Findymail
provider_slug: findymail
slug: findymail-domain-security
source_filename: findymail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findymail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 17:48:07 2027 GMT\n  hsts: null\ndomains:\n- domain: findymail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/findymail/security/findymail-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email Finder
- B2B Data
- Lead Generation
---
