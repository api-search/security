---
api_specs:
- filename: puma-openapi.yml
  format: yaml
  label: Puma Control/Status Application
  slug: control-app
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: puma.io
  spf: true
hosts:
- cert_expires: Sep 27 20:00:51 2026 GMT
  host: puma.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Puma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Puma, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Puma
provider_slug: puma
slug: puma-domain-security
source_filename: puma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: puma.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 20:00:51 2026 GMT\n  hsts: false\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: puma.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/security/puma-domain-security.yml
summary_line: TLSv1.3
tags:
- Web Server
- Ruby
- Rack
- Application Server
- HTTP
- Open Source
---
