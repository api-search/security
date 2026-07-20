---
api_specs:
- filename: coronet-webhooks-asyncapi.yml
  format: yaml
  label: Coro Public API
  slug: coro-public-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/coronet/refs/heads/main/asyncapi/coronet-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coro.net
  spf: true
hosts:
- cert_expires: Sep 14 08:00:52 2026 GMT
  host: www.coro.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 10:55:13 2026 GMT
  host: docs.coro.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: api.secure.coro.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coronet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoroNet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CoroNet
provider_slug: coronet
slug: coronet-domain-security
source_filename: coronet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coro.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:00:52 2026 GMT\n  hsts: false\n- host: docs.coro.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 10:55:13 2026 GMT\n  hsts: false\n- host: api.secure.coro.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coro.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coronet/refs/heads/main/security/coronet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Cybersecurity
- Security
- Endpoint Security
- Email Security
- Network Security
- Cloud Security
- Managed Service Providers
- Compliance
- Webhooks
- API
---
