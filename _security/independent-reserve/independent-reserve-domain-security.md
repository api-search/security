---
api_specs:
- filename: independent-reserve-private-api-openapi.yml
  format: yaml
  label: Independent Reserve Private API
  slug: independent-reserve-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independent-reserve/refs/heads/main/openapi/independent-reserve-private-api-openapi.yml
- filename: independent-reserve-public-api-openapi.yml
  format: yaml
  label: Independent Reserve Public API
  slug: independent-reserve-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independent-reserve/refs/heads/main/openapi/independent-reserve-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: independentreserve.com
  spf: true
hosts:
- cert_expires: Dec  1 10:14:07 2026 GMT
  host: www.independentreserve.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Independent Reserve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Independent Reserve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Independent Reserve
provider_slug: independent-reserve
slug: independent-reserve-domain-security
source_filename: independent-reserve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.independentreserve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 10:14:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: independentreserve.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/independent-reserve/refs/heads/main/security/independent-reserve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Bitcoin
- Financial Services
---
