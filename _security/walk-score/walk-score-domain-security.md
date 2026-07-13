---
api_specs:
- filename: walk-score-openapi.yml
  format: yaml
  label: Walk Score API
  slug: walk-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walk-score/refs/heads/main/openapi/walk-score-openapi.yml
- filename: walk-score-transit-openapi.yml
  format: yaml
  label: Walk Score Transit API
  slug: walk-score-transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walk-score/refs/heads/main/openapi/walk-score-transit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: walkscore.com
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: www.walkscore.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  9 06:05:02 2026 GMT
  host: api.walkscore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 08:16:03 2026 GMT
  host: transit.walkscore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Walk Score Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Walk Score, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Walk Score
provider_slug: walk-score
slug: walk-score-domain-security
source_filename: walk-score-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.walkscore.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.walkscore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 06:05:02 2026 GMT\n  hsts: false\n- host: transit.walkscore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:16:03 2026 GMT\n  hsts: false\ndomains:\n- domain: walkscore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walk-score/refs/heads/main/security/walk-score-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Walkability
- Transit
- Bikeability
- Location
- Real Estate
- Urban Planning
- Transportation
---
