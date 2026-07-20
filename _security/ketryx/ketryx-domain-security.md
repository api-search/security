---
api_specs:
- filename: ketryx-build-api-openapi.yml
  format: yaml
  label: Ketryx Build API
  slug: ketryx-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ketryx/refs/heads/main/openapi/ketryx-build-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ketryx.com
  spf: true
hosts:
- cert_expires: Sep 17 10:52:08 2026 GMT
  host: docs.ketryx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: app.ketryx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ketryx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ketryx, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ketryx
provider_slug: ketryx
slug: ketryx-domain-security
source_filename: ketryx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.ketryx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 10:52:08 2026 GMT\n  hsts: null\n- host: app.ketryx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ketryx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ketryx/refs/heads/main/security/ketryx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Life Sciences
- Compliance
- Regulatory
- Application Lifecycle Management
- Quality Management
- SBOM
- DevOps
- Healthcare
- Governance
- CI/CD
---
