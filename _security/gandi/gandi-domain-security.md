---
api_specs:
- filename: domains-openapi-original.yml
  format: yaml
  label: Gandi Domain API
  slug: domains
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/domains-openapi-original.yml
- filename: livedns-openapi-original.yml
  format: yaml
  label: Gandi LiveDNS API
  slug: livedns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/livedns-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gandi.net
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: www.gandi.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.gandi.net
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.sandbox.gandi.net
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gandi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gandi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gandi
provider_slug: gandi
slug: gandi-domain-security
source_filename: gandi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gandi.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gandi.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.sandbox.gandi.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: gandi.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/security/gandi-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- DNS
- Domains
- Domain Registrar
- Email
- Hosting
- Certificates
---
