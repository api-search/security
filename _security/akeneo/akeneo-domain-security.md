---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Akeneo PIM REST API
  slug: pim-rest-api
  spec_type: OpenAPI
  url: https://storage.googleapis.com/akecld-prd-pim-saas-shared-openapi-spec/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: akeneo.com
  spf: true
hosts:
- cert_expires: Aug 18 13:59:22 2026 GMT
  host: www.akeneo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:34:56 2026 GMT
  host: api.akeneo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akeneo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akeneo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Akeneo
provider_slug: akeneo
slug: akeneo-domain-security
source_filename: akeneo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akeneo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:59:22 2026 GMT\n  hsts: false\n- host: api.akeneo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:34:56 2026 GMT\n  hsts: false\ndomains:\n- domain: akeneo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/security/akeneo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Product Information Management
- PIM
- Product Data
- Catalog Management
- Commerce
- Retail
---
