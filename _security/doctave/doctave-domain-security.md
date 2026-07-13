---
api_specs:
- filename: doctave-doctave-openapi.yml
  format: yaml
  label: Doctave API
  slug: doctave
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doctave/refs/heads/main/openapi/doctave-doctave-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doctave.com
  spf: false
hosts:
- cert_expires: Sep 28 11:16:24 2026 GMT
  host: www.doctave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.doctave.com
  https: false
kind: domain-security
layout: security
method: probed
name: Doctave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doctave, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Doctave
provider_slug: doctave
slug: doctave-domain-security
source_filename: doctave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doctave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:16:24 2026 GMT\n  hsts: false\n- host: api.doctave.com\n  https: false\ndomains:\n- domain: doctave.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doctave/refs/heads/main/security/doctave-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Documentation
- OpenAPI
- Platform
- Portals
---
