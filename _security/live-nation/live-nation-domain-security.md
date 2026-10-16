---
api_specs:
- filename: live-nation-openapi-generated.yml
  format: yaml
  label: Live Nation API
  slug: live-nation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-nation/refs/heads/main/openapi/_ae-authored/live-nation-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: livenation.com
  spf: true
hosts:
- cert_expires: Nov 29 17:01:36 2026 GMT
  host: www.livenation.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Live Nation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Live Nation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Live Nation
provider_slug: live-nation
slug: live-nation-domain-security
source_filename: live-nation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.livenation.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 17:01:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: livenation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/live-nation/refs/heads/main/security/live-nation-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Entertainment
- Ticketing
- Live Events
- Music
- Technology
---
