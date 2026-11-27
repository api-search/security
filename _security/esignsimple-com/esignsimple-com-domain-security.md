---
api_specs:
- filename: esignsimple-com-account-api-openapi.yml
  format: yaml
  label: eSignSimple Account API
  slug: esignsimple-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esignsimple-com/openapi/esignsimple-com-account-api-openapi.yml
- filename: esignsimple-com-documents-api-openapi.yml
  format: yaml
  label: eSignSimple Documents API
  slug: esignsimple-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esignsimple-com/openapi/esignsimple-com-documents-api-openapi.yml
- filename: esignsimple-com-templates-api-openapi.yml
  format: yaml
  label: eSignSimple Templates API
  slug: esignsimple-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esignsimple-com/openapi/esignsimple-com-templates-api-openapi.yml
- filename: esignsimple-com-verification-api-openapi.yml
  format: yaml
  label: eSignSimple Verification API
  slug: esignsimple-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esignsimple-com/openapi/esignsimple-com-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: esignsimple.com
  spf: true
hosts:
- cert_expires: Dec 22 20:39:14 2026 GMT
  host: esignsimple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: eSignSimple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eSignSimple, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: eSignSimple
provider_slug: esignsimple-com
slug: esignsimple-com-domain-security
source_filename: esignsimple-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: esignsimple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 20:39:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: esignsimple.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/esignsimple-com/security/esignsimple-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Signature
- Templates
- Bulk Sending
- Web Forms
- ID Verification
---
