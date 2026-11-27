---
api_specs:
- filename: evaboot-com-account-api-openapi.yml
  format: yaml
  label: Evaboot Account API
  slug: evaboot-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evaboot-com/openapi/evaboot-com-account-api-openapi.yml
- filename: evaboot-com-email-finder-api-openapi.yml
  format: yaml
  label: Evaboot Email Finder API
  slug: evaboot-com-email-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evaboot-com/openapi/evaboot-com-email-finder-api-openapi.yml
- filename: evaboot-com-email-verifier-api-openapi.yml
  format: yaml
  label: Evaboot Email Verifier API
  slug: evaboot-com-email-verifier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evaboot-com/openapi/evaboot-com-email-verifier-api-openapi.yml
- filename: evaboot-com-linkedin-extraction-api-openapi.yml
  format: yaml
  label: Evaboot LinkedIn Extraction API
  slug: evaboot-com-linkedin-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evaboot-com/openapi/evaboot-com-linkedin-extraction-api-openapi.yml
- filename: evaboot-com-search-builder-api-openapi.yml
  format: yaml
  label: Evaboot Search Builder API
  slug: evaboot-com-search-builder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evaboot-com/openapi/evaboot-com-search-builder-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: evaboot.com
  spf: true
hosts:
- cert_expires: Dec 30 09:48:58 2026 GMT
  host: evaboot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Evaboot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evaboot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Evaboot
provider_slug: evaboot-com
slug: evaboot-com-domain-security
source_filename: evaboot-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evaboot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 09:48:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: evaboot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/evaboot-com/security/evaboot-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Lead Generation
- Sales
- Data Cleaning
- Email Verification
- Chrome Extension
---
