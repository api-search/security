---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apisjson.org
  spf: false
hosts:
- cert_expires: Sep 14 08:02:26 2026 GMT
  host: apisjson.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apis Json Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIs.json, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: APIs.json
provider_slug: apis-json
slug: apis-json-domain-security
source_filename: apis-json-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apisjson.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:02:26 2026 GMT\n  hsts: false\ndomains:\n- domain: apisjson.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-json/refs/heads/main/security/apis-json-domain-security.yml
summary_line: TLSv1.3
tags:
- API Aggregation
- API Cataloging
- API Commons
- API Discovery
- API Governance
- API Operations
- Machine Readable
- Specification
- Standard
---
