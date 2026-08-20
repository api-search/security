---
api_specs:
- filename: pulse-software-authentication-api-openapi.yml
  format: yaml
  label: Pulse Software Authentication API
  slug: pulse-software-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-authentication-api-openapi.yml
- filename: pulse-software-corporate-planning-api-api-openapi.yml
  format: yaml
  label: Pulse Software Corporate Planning API API
  slug: pulse-software-corporate-planning-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-corporate-planning-api-api-openapi.yml
- filename: pulse-software-forms-api-api-openapi.yml
  format: yaml
  label: Pulse Software Forms API API
  slug: pulse-software-forms-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-forms-api-api-openapi.yml
- filename: pulse-software-learning-api-api-openapi.yml
  format: yaml
  label: Pulse Software Learning API API
  slug: pulse-software-learning-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-learning-api-api-openapi.yml
- filename: pulse-software-project-api-api-openapi.yml
  format: yaml
  label: Pulse Software Project API API
  slug: pulse-software-project-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-project-api-api-openapi.yml
- filename: pulse-software-recruitment-api-api-openapi.yml
  format: yaml
  label: Pulse Software Recruitment API API
  slug: pulse-software-recruitment-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-recruitment-api-api-openapi.yml
- filename: pulse-software-sync-api-api-openapi.yml
  format: yaml
  label: Pulse Software Sync API API
  slug: pulse-software-sync-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-sync-api-api-openapi.yml
- filename: pulse-software-user-details-api-api-openapi.yml
  format: yaml
  label: Pulse Software User Details API API
  slug: pulse-software-user-details-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-user-details-api-api-openapi.yml
- filename: pulse-software-user-details-api-v2-api-openapi.yml
  format: yaml
  label: Pulse Software User Details API v2 API
  slug: pulse-software-user-details-api-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-user-details-api-v2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pulsesoftware.com
  spf: true
hosts:
- cert_expires: Sep  2 07:34:03 2026 GMT
  host: apidoc.pulsesoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: '*.pulsesoftware.com'
  https: false
kind: domain-security
layout: security
method: probed
name: Pulse Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulse Software, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pulse Software
provider_slug: pulse-software
slug: pulse-software-domain-security
source_filename: pulse-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apidoc.pulsesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 07:34:03 2026 GMT\n  hsts: false\n- host: '*.pulsesoftware.com'\n  https: false\ndomains:\n- domain: pulsesoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/security/pulse-software-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pulse
- Automation
- Developers
---
