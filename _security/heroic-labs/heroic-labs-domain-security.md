---
api_specs:
- filename: heroic-labs-nakama-openapi-original.json
  format: json
  label: Nakama API v2
  slug: nakama-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroic-labs/refs/heads/main/openapi/heroic-labs-nakama-openapi-original.json
- filename: heroic-labs-nakama-console-openapi-original.json
  format: json
  label: Nakama Console API v2
  slug: nakama-console-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroic-labs/refs/heads/main/openapi/heroic-labs-nakama-console-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: heroiclabs.com
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: heroiclabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: cloud.heroiclabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Heroic Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heroic Labs, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Heroic Labs
provider_slug: heroic-labs
slug: heroic-labs-domain-security
source_filename: heroic-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heroiclabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\n- host: cloud.heroiclabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: heroiclabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heroic-labs/refs/heads/main/security/heroic-labs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Gaming
- Game Backend
- Multiplayer
- Real-Time
- LiveOps
- Open Source
- Developer Tools
- Backend as a Service
---
