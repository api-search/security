---
api_specs:
- filename: dragos-worldview-openapi-original.json
  format: json
  label: Dragos WorldView API
  slug: dragos-worldview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dragos/refs/heads/main/openapi/dragos-worldview-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dragos.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dragos.cloud
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: portal.dragos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: www.dragos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: platform.dragos.cloud
  https: false
kind: domain-security
layout: security
method: probed
name: Dragos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dragos, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dragos
provider_slug: dragos
slug: dragos-domain-security
source_filename: dragos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.dragos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.dragos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.dragos.cloud\n  https: false\ndomains:\n- domain: dragos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dragos.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dragos/refs/heads/main/security/dragos-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- OT Security
- ICS
- Threat Intelligence
- Industrial Control Systems
- Indicators of Compromise
- STIX
- Vulnerability Management
- Security
---
