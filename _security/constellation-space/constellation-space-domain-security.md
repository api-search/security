---
api_specs:
- filename: constellation-space-openapi.yml
  format: yaml
  label: ConstellationOS API
  slug: constellationos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-space/refs/heads/main/openapi/constellation-space-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: constellation.space
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: constellation.space
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: docs.constellation.space
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: api.constellation.space
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Constellation Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constellation Space, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Constellation Space
provider_slug: constellation-space
slug: constellation-space-domain-security
source_filename: constellation-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: constellation.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n- host: docs.constellation.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: api.constellation.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: constellation.space\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constellation-space/refs/heads/main/security/constellation-space-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Satellites
- Space
- Telemetry
- Machine Learning
- Fleet Operations
- Ground Segment
- Predictions
---
