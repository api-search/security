---
api_specs:
- filename: eppo-openapi.yml
  format: yaml
  label: Eppo Cloud REST API
  slug: eppo-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eppo/refs/heads/main/openapi/eppo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: geteppo.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: eppo.cloud
  spf: false
hosts:
- cert_expires: Aug 17 07:33:18 2026 GMT
  host: www.geteppo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 17:42:40 2026 GMT
  host: eppo.cloud
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eppo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eppo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eppo
provider_slug: eppo
slug: eppo-domain-security
source_filename: eppo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geteppo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 07:33:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eppo.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:42:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: geteppo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eppo.cloud\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eppo/refs/heads/main/security/eppo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Experimentation
- Feature Flags
- AB Testing
- Analytics
- Statistics
---
