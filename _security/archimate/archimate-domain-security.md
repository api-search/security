---
api_specs:
- filename: archimate-model-exchange-api.yaml
  format: yaml
  label: ArchiMate Model Exchange API
  slug: archimate-model-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/openapi/archimate-model-exchange-api.yaml
- filename: archimate-repository-api.yaml
  format: yaml
  label: ArchiMate Repository API
  slug: archimate-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/openapi/archimate-repository-api.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opengroup.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: archimate-tools.com
  spf: false
hosts:
- cert_expires: Oct 22 19:06:18 2026 GMT
  host: www.opengroup.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.archimate-tools.com
  https: false
kind: domain-security
layout: security
method: probed
name: Archimate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ArchiMate, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ArchiMate
provider_slug: archimate
slug: archimate-domain-security
source_filename: archimate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opengroup.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 19:06:18 2026 GMT\n  hsts: false\n- host: api.archimate-tools.com\n  https: false\ndomains:\n- domain: opengroup.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: archimate-tools.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/security/archimate-domain-security.yml
summary_line: TLSv1.3
tags:
- Enterprise Architecture
- Architecture Framework
- Modeling Language
- Business Architecture
- Technology Architecture
- Standard
- Open Group
---
