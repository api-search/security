---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spiritaero.com
  spf: true
hosts:
- cert_expires: Jul 20 14:54:14 2026 GMT
  host: www.spiritaero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spirit Aerosystems Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spirit AeroSystems Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spirit AeroSystems Holdings
provider_slug: spirit-aerosystems-holdings
slug: spirit-aerosystems-holdings-domain-security
source_filename: spirit-aerosystems-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spiritaero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 20 14:54:14 2026 GMT\n  hsts: false\ndomains:\n- domain: spiritaero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spirit-aerosystems-holdings/refs/heads/main/security/spirit-aerosystems-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aerospace
- Aerostructures
- Defense
- Manufacturing
- Fortune 500
---
