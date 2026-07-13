---
api_specs:
- filename: cms-energy-openapi.yml
  format: yaml
  label: Consumers Energy Green Button Connect My Data API
  slug: consumers-green-button-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cmsenergy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: consumersenergy.com
  spf: true
hosts:
- cert_expires: Aug 26 14:48:40 2026 GMT
  host: www.cmsenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: www.consumersenergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 19:11:25 2026 GMT
  host: utilityapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cms Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CMS Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CMS Energy
provider_slug: cms-energy
slug: cms-energy-domain-security
source_filename: cms-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cmsenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:48:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.consumersenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\n- host: utilityapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 19:11:25 2026 GMT\n  hsts: false\ndomains:\n- domain: cmsenergy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: consumersenergy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/security/cms-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Electric
- Energy
- Green Button
- Michigan
- Natural Gas
- Utility
- Fortune 500
---
