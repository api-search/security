---
api_specs:
- filename: airspace-technologies-v3-openapi.json
  format: json
  label: Airspace API V3
  slug: airspace-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airspace-technologies/refs/heads/main/openapi/airspace-technologies-v3-openapi.json
- filename: airspace-technologies-v2-openapi.json
  format: json
  label: Airspace API V2
  slug: airspace-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airspace-technologies/refs/heads/main/openapi/airspace-technologies-v2-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airspace.com
  spf: true
hosts:
- cert_expires: Oct 14 18:44:41 2026 GMT
  host: www.airspace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 08:27:24 2026 GMT
  host: api.airspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airspace Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airspace Technologies, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airspace Technologies
provider_slug: airspace-technologies
slug: airspace-technologies-domain-security
source_filename: airspace-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:44:41 2026 GMT\n  hsts: false\n- host: api.airspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 08:27:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: airspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airspace-technologies/refs/heads/main/security/airspace-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Shipping
- Freight
- Supply Chain
- Transportation
- Webhooks
- Orders
---
