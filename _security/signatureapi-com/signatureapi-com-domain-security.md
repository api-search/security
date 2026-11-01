---
api_specs:
- filename: signatureapi-com-deliverables-api-openapi.yml
  format: yaml
  label: signatureapi-com Deliverables API
  slug: signatureapi-com-deliverables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-deliverables-api-openapi.yml
- filename: signatureapi-com-envelopes-api-openapi.yml
  format: yaml
  label: signatureapi-com Envelopes API
  slug: signatureapi-com-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-envelopes-api-openapi.yml
- filename: signatureapi-com-events-api-openapi.yml
  format: yaml
  label: signatureapi-com Events API
  slug: signatureapi-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-events-api-openapi.yml
- filename: signatureapi-com-recipients-api-openapi.yml
  format: yaml
  label: signatureapi-com Recipients API
  slug: signatureapi-com-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-recipients-api-openapi.yml
- filename: signatureapi-com-senders-api-openapi.yml
  format: yaml
  label: signatureapi-com Senders API
  slug: signatureapi-com-senders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-senders-api-openapi.yml
- filename: signatureapi-com-uploads-api-openapi.yml
  format: yaml
  label: signatureapi-com Uploads API
  slug: signatureapi-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-uploads-api-openapi.yml
- filename: signatureapi-com-webhooks-api-openapi.yml
  format: yaml
  label: signatureapi-com Webhooks API
  slug: signatureapi-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: signatureapi.com
  spf: true
hosts:
- cert_expires: Jan 25 16:32:49 2027 GMT
  host: signatureapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Signatureapi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for signatureapi-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: signatureapi-com
provider_slug: signatureapi-com
slug: signatureapi-com-domain-security
source_filename: signatureapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signatureapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 16:32:49 2027 GMT\n  hsts: false\ndomains:\n- domain: signatureapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/signatureapi-com/security/signatureapi-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- ElectronicSignature
- API
- SaaS
- Compliance
- Automation
---
