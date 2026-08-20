---
api_specs:
- filename: puma-gc-api-openapi.yml
  format: yaml
  label: Puma Gc API
  slug: puma-gc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-gc-api-openapi.yml
- filename: puma-gc-stats-api-openapi.yml
  format: yaml
  label: Puma Gc Stats API
  slug: puma-gc-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-gc-stats-api-openapi.yml
- filename: puma-halt-api-openapi.yml
  format: yaml
  label: Puma Halt API
  slug: puma-halt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-halt-api-openapi.yml
- filename: puma-phased-restart-api-openapi.yml
  format: yaml
  label: Puma Phased Restart API
  slug: puma-phased-restart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-phased-restart-api-openapi.yml
- filename: puma-refork-api-openapi.yml
  format: yaml
  label: Puma Refork API
  slug: puma-refork-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-refork-api-openapi.yml
- filename: puma-reload-worker-directory-api-openapi.yml
  format: yaml
  label: Puma Reload Worker Directory API
  slug: puma-reload-worker-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-reload-worker-directory-api-openapi.yml
- filename: puma-restart-api-openapi.yml
  format: yaml
  label: Puma Restart API
  slug: puma-restart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-restart-api-openapi.yml
- filename: puma-stats-api-openapi.yml
  format: yaml
  label: Puma Stats API
  slug: puma-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-stats-api-openapi.yml
- filename: puma-stop-api-openapi.yml
  format: yaml
  label: Puma Stop API
  slug: puma-stop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-stop-api-openapi.yml
- filename: puma-thread-backtraces-api-openapi.yml
  format: yaml
  label: Puma Thread Backtraces API
  slug: puma-thread-backtraces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-thread-backtraces-api-openapi.yml
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
- Open-Source
---
