---
description: ''
domains:
- caa:
  - 0 iodef "mailto:admin@pack.io"
  - 0 issuewild "sectigo.com"
  dmarc: false
  dnssec: true
  domain: pack.io
  spf: false
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: pack.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pack Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Pack
provider_slug: pack-io
slug: pack-io-domain-security
source_filename: pack-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pack.io\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:admin@pack.io\"\n  - 0 issuewild \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pack-io/security/pack-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Technology
- Packaging
- API
- Startup
---
