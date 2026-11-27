---
api_specs:
- filename: medsender-ai-documents-api-openapi.yml
  format: yaml
  label: Medsender AI Documents API
  slug: medsender-ai-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-ai-documents-api-openapi.yml
- filename: medsender-clients-api-openapi.yml
  format: yaml
  label: Medsender Clients API
  slug: medsender-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-clients-api-openapi.yml
- filename: medsender-fax-numbers-api-openapi.yml
  format: yaml
  label: Medsender Fax Numbers API
  slug: medsender-fax-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-fax-numbers-api-openapi.yml
- filename: medsender-received-faxes-api-openapi.yml
  format: yaml
  label: Medsender Received Faxes API
  slug: medsender-received-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-received-faxes-api-openapi.yml
- filename: medsender-secure-links-api-openapi.yml
  format: yaml
  label: Medsender Secure Links API
  slug: medsender-secure-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-secure-links-api-openapi.yml
- filename: medsender-sent-faxes-api-openapi.yml
  format: yaml
  label: Medsender Sent Faxes API
  slug: medsender-sent-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-sent-faxes-api-openapi.yml
- filename: medsender-v3-fax-numbers-api-openapi.yml
  format: yaml
  label: Medsender V3 Fax Numbers API
  slug: medsender-v3-fax-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-v3-fax-numbers-api-openapi.yml
- filename: medsender-v3-received-faxes-api-openapi.yml
  format: yaml
  label: Medsender V3 Received Faxes API
  slug: medsender-v3-received-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-v3-received-faxes-api-openapi.yml
- filename: medsender-v3-sent-faxes-api-openapi.yml
  format: yaml
  label: Medsender V3 Sent Faxes API
  slug: medsender-v3-sent-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-v3-sent-faxes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medsender.com
  spf: true
hosts:
- cert_expires: Feb  9 16:59:29 2027 GMT
  host: medsender.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Medsender Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medsender, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Medsender
provider_slug: medsender
slug: medsender-domain-security
source_filename: medsender-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medsender.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 16:59:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: medsender.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/medsender/security/medsender-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Referral Management
- Fax Automation
- Patient Recapture
- Call Automation
- EHR Integration
---
