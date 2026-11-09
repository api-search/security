---
api_specs:
- filename: anchoredip-com-openapi-generated.yml
  format: yaml
  label: AnchoredIP API
  slug: anchoredip-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchoredip-com/openapi/_ae-authored/anchoredip-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:oleg@iptech.kz"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: anchoredip.com
  spf: true
hosts:
- cert_expires: Dec 22 22:16:57 2026 GMT
  host: anchoredip.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anchoredip Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnchoredIP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: AnchoredIP
provider_slug: anchoredip-com
slug: anchoredip-com-domain-security
source_filename: anchoredip-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anchoredip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 22:16:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anchoredip.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:oleg@iptech.kz\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/anchoredip-com/security/anchoredip-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- StaticIP
- Networking
- Cloud
- WireGuard
- Outbound
---
