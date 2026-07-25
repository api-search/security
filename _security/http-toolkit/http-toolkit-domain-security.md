---
api_specs:
- filename: http-toolkit-client-api-openapi.yml
  format: yaml
  label: HTTP Toolkit client API
  slug: http-toolkit-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/http-toolkit/refs/heads/main/openapi/http-toolkit-client-api-openapi.yml
- filename: http-toolkit-config-api-openapi.yml
  format: yaml
  label: HTTP Toolkit config API
  slug: http-toolkit-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/http-toolkit/refs/heads/main/openapi/http-toolkit-config-api-openapi.yml
- filename: http-toolkit-interceptors-api-openapi.yml
  format: yaml
  label: HTTP Toolkit interceptors API
  slug: http-toolkit-interceptors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/http-toolkit/refs/heads/main/openapi/http-toolkit-interceptors-api-openapi.yml
- filename: http-toolkit-server-api-openapi.yml
  format: yaml
  label: HTTP Toolkit server API
  slug: http-toolkit-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/http-toolkit/refs/heads/main/openapi/http-toolkit-server-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: httptoolkit.com
  spf: true
hosts:
- cert_expires: Sep 18 02:01:54 2026 GMT
  host: httptoolkit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Http Toolkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HTTP Toolkit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HTTP Toolkit
provider_slug: http-toolkit
slug: http-toolkit-domain-security
source_filename: http-toolkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: httptoolkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:01:54 2026 GMT\n  hsts: false\ndomains:\n- domain: httptoolkit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/http-toolkit/refs/heads/main/security/http-toolkit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- HTTP
- HTTPS
- Debugging
- Proxy
- Interception
- Mocking
- Testing
- Developer Tools
- Open Source
---
