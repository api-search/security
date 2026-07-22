---
api_specs:
- filename: tidelift-subscriber-api-openapi-original.json
  format: json
  label: Tidelift External API
  slug: tidelift-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-subscriber-api-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tidelift.com
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.tidelift.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tidelift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tidelift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tidelift
provider_slug: tidelift
slug: tidelift-domain-security
source_filename: tidelift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.tidelift.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tidelift.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/security/tidelift-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Open Source
- Software Supply Chain
- Dependency Management
- Application Security
- SBOM
- License Compliance
- Vulnerability Management
- Developer Tools
---
