---
api_specs:
- filename: vessel-platform-openapi.yml
  format: yaml
  label: Vessel Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-platform-openapi.yml
- filename: vessel-crm-openapi.yml
  format: yaml
  label: Vessel CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-crm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vessel.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vessel.land
  spf: true
hosts:
- cert_expires: Oct  1 06:58:09 2026 GMT
  host: www.vessel.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.vessel.land
  https: false
- cert_expires: Aug 16 11:23:53 2026 GMT
  host: api.vessel.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vessel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vessel, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vessel
provider_slug: vessel
slug: vessel-domain-security
source_filename: vessel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vessel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:58:09 2026 GMT\n  hsts: false\n- host: api.vessel.land\n  https: false\n- host: api.vessel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:23:53 2026 GMT\n  hsts: null\ndomains:\n- domain: vessel.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: vessel.land\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/security/vessel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Embedded Integrations
- GTM
- Integrations
- iPaaS
- Sales Engagement
- Unified API
---
