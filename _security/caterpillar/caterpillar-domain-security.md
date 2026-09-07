---
api_specs:
- filename: iso-15143-3-aemp-20-api-postman-collection
  format: yaml
  label: ISO 15143-3 (AEMP 2.0) API
  slug: iso-15143-3-aemp-api
  spec_type: Postman
  url: https://digital.cat.com/knowledge-hub/document/iso-15143-3-aemp-20-api-postman-collection
- filename: visionlink-apis-postman-collection
  format: yaml
  label: VisionLink APIs
  slug: visionlink-apis
  spec_type: Postman
  url: https://digital.cat.com/knowledge-hub/document/visionlink-apis-postman-collection
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "www.digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: caterpillar.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cat.com
  spf: true
hosts:
- cert_expires: Oct 21 14:33:30 2026 GMT
  host: www.caterpillar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: digital.cat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: services.cat.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Caterpillar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caterpillar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Caterpillar
provider_slug: caterpillar
slug: caterpillar-domain-security
source_filename: caterpillar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caterpillar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 14:33:30 2026 GMT\n  hsts: null\n- host: digital.cat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.cat.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: caterpillar.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"www.digicert.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: cat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caterpillar/refs/heads/main/security/caterpillar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Engines
- Fortune 500
- Heavy Equipment
- Locomotives
- Manufacturing
- Mining
- Telematics
- Fleet Management
- ISO 15143-3
- AEMP
---
