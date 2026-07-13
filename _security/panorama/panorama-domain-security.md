---
api_specs:
- filename: panorama-openapi.yml
  format: yaml
  label: Panorama API
  slug: panorama
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panorama/refs/heads/main/openapi/panorama-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: paloaltonetworks.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.paloaltonetworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 20:15:31 2026 GMT
  host: docs.paloaltonetworks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Panorama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panorama, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Panorama
provider_slug: panorama
slug: panorama-domain-security
source_filename: panorama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paloaltonetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.paloaltonetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 20:15:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: paloaltonetworks.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panorama/refs/heads/main/security/panorama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Firewall Management
- Network Security
- Palo Alto Networks
---
