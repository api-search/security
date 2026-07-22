---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:admin@technipfmc.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: technipfmc.com
  spf: true
hosts:
- cert_expires: Sep 15 06:04:43 2026 GMT
  host: www.technipfmc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fmc Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FMC Technologies (now TechnipFMC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FMC Technologies (now TechnipFMC)
provider_slug: fmc-technologies
slug: fmc-technologies-domain-security
source_filename: fmc-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.technipfmc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:04:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: technipfmc.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:admin@technipfmc.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fmc-technologies/refs/heads/main/security/fmc-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Oil and Gas
- Subsea
- Industrial
- Fortune 1000
---
