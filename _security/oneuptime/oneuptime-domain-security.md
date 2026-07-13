---
api_specs:
- filename: oneuptime-openapi.yml
  format: yaml
  label: OneUptime
  slug: oneuptime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneuptime/refs/heads/main/openapi/oneuptime-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: oneuptime.com
  spf: true
hosts:
- cert_expires: Sep  7 14:39:34 2026 GMT
  host: oneuptime.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oneuptime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneUptime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: OneUptime
provider_slug: oneuptime
slug: oneuptime-domain-security
source_filename: oneuptime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oneuptime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:39:34 2026 GMT\n  hsts: false\ndomains:\n- domain: oneuptime.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneuptime/refs/heads/main/security/oneuptime-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Observability
- Open Source
---
