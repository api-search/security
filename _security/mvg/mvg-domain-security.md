---
description: ''
domains:
- caa:
  - 0 issue "telesec.de"
  - 0 iodef "mailto:support.web@swm.de"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mvg.de
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: mvg.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mvg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MVG (Munich transit), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MVG (Munich transit)
provider_slug: mvg
slug: mvg-domain-security
source_filename: mvg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mvg.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mvg.de\n  dnssec: false\n  caa:\n  - 0 issue \"telesec.de\"\n  - 0 iodef \"mailto:support.web@swm.de\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mvg/security/mvg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Transportation
- PublicTransit
- Munich
- Germany
---
