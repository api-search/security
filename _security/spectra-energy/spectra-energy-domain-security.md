---
description: ''
domains:
- caa:
  - 128 iodef "mailto:pkisupport@enbridge.com"
  - 128 issue "digicert.com"
  - 128 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: enbridge.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.enbridge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spectra Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spectra Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spectra Energy
provider_slug: spectra-energy
slug: spectra-energy-domain-security
source_filename: spectra-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enbridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: enbridge.com\n  dnssec: true\n  caa:\n  - 128 iodef \"mailto:pkisupport@enbridge.com\"\n  - 128 issue \"digicert.com\"\n  - 128 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spectra-energy/refs/heads/main/security/spectra-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Natural Gas
- Oil and Gas
- Pipeline
- Utilities
- Fortune 500
---
