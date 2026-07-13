---
api_specs:
- filename: guidewire-policycenter-openapi.yml
  format: yaml
  label: Guidewire PolicyCenter API
  slug: guidewire-policycenter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-policycenter-openapi.yml
- filename: guidewire-claimcenter-openapi.yml
  format: yaml
  label: Guidewire ClaimCenter API
  slug: guidewire-claimcenter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-claimcenter-openapi.yml
- filename: guidewire-integration-gateway-asyncapi.yml
  format: yaml
  label: Guidewire Integration Gateway API
  slug: guidewire-integration-gateway-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/asyncapi/guidewire-integration-gateway-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "starfieldtech.com"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: guidewire.com
  spf: true
hosts:
- cert_expires: Oct  9 06:21:21 2026 GMT
  host: docs.guidewire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.guidewire.com
  https: false
kind: domain-security
layout: security
method: probed
name: Guidewire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guidewire, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Guidewire
provider_slug: guidewire
slug: guidewire-domain-security
source_filename: guidewire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.guidewire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 06:21:21 2026 GMT\n  hsts: false\n- host: api.guidewire.com\n  https: false\ndomains:\n- domain: guidewire.com\n  dnssec: false\n  caa:\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/security/guidewire-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Policy
- Claims
- Billing
- P&C
---
