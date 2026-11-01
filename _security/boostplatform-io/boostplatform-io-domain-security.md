---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boostplatform.io
  spf: true
hosts:
- cert_expires: Dec  1 22:18:41 2026 GMT
  host: www.boostplatform.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boostplatform Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boost Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boost Insurance
provider_slug: boostplatform-io
slug: boostplatform-io-domain-security
source_filename: boostplatform-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boostplatform.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 22:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boostplatform.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/boostplatform-io/security/boostplatform-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance Platform
- Insurtech
- MGA
- Embedded Insurance
- API
---
