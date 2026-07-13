---
api_specs:
- filename: betsolutions-wallet-api.yaml
  format: yaml
  label: BetSolutions Wallet API
  slug: wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/openapi/betsolutions-wallet-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: betsolutions.com
  spf: true
hosts:
- cert_expires: Sep 20 19:00:55 2026 GMT
  host: betsolutions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 19:00:55 2026 GMT
  host: docs.betsolutions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 19:00:55 2026 GMT
  host: api.betsolutions.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betsolutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetSolutions, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BetSolutions
provider_slug: betsolutions
slug: betsolutions-domain-security
source_filename: betsolutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:00:55 2026 GMT\n  hsts: false\n- host: docs.betsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:00:55 2026 GMT\n  hsts: false\n- host: api.betsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:00:55 2026 GMT\n  hsts: null\ndomains:\n- domain: betsolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/security/betsolutions-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
---
