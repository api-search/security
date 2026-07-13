---
api_specs:
- filename: thermal-power-openapi.yml
  format: yaml
  label: Thermal Power API
  slug: thermal-power
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermal-power/refs/heads/main/openapi/thermal-power-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eia.gov
  spf: true
hosts:
- cert_expires: Aug 19 23:59:59 2026 GMT
  host: www.eia.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 17:20:52 2026 GMT
  host: api.eia.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thermal Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thermal Power, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Thermal Power
provider_slug: thermal-power
slug: thermal-power-domain-security
source_filename: thermal-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.eia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:20:52 2026 GMT\n  hsts: null\ndomains:\n- domain: eia.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thermal-power/refs/heads/main/security/thermal-power-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Energy
- Thermal Power
- Power Generation
- Electricity
- Coal
- Natural Gas
- Nuclear
---
