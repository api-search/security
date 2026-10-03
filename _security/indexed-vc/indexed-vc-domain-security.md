---
api_specs:
- filename: indexed-vc-companies-api-openapi.yml
  format: yaml
  label: Indexed Companies API
  slug: indexed-vc-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-companies-api-openapi.yml
- filename: indexed-vc-enrich-api-openapi.yml
  format: yaml
  label: Indexed Enrich API
  slug: indexed-vc-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-enrich-api-openapi.yml
- filename: indexed-vc-industries-api-openapi.yml
  format: yaml
  label: Indexed Industries API
  slug: indexed-vc-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-industries-api-openapi.yml
- filename: indexed-vc-investors-api-openapi.yml
  format: yaml
  label: Indexed Investors API
  slug: indexed-vc-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-investors-api-openapi.yml
- filename: indexed-vc-reveal-api-openapi.yml
  format: yaml
  label: Indexed Reveal API
  slug: indexed-vc-reveal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-reveal-api-openapi.yml
- filename: indexed-vc-scheduled-exports-api-openapi.yml
  format: yaml
  label: Indexed Scheduled Exports API
  slug: indexed-vc-scheduled-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-scheduled-exports-api-openapi.yml
- filename: indexed-vc-usage-api-openapi.yml
  format: yaml
  label: Indexed Usage API
  slug: indexed-vc-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-usage-api-openapi.yml
- filename: indexed-vc-webhooks-api-openapi.yml
  format: yaml
  label: Indexed Webhooks API
  slug: indexed-vc-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: indexed.vc
  spf: true
hosts:
- cert_expires: Dec  4 03:33:23 2026 GMT
  host: indexed.vc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Indexed Vc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indexed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Indexed
provider_slug: indexed-vc
slug: indexed-vc-domain-security
source_filename: indexed-vc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indexed.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 03:33:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: indexed.vc\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/security/indexed-vc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Private Company
- Funding
---
