---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: powerlighttech.com
  spf: true
hosts:
- cert_expires: Oct 21 06:09:03 2026 GMT
  host: powerlighttech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powerlight Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PowerLight Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PowerLight Technologies
provider_slug: powerlight-technologies
slug: powerlight-technologies-domain-security
source_filename: powerlight-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: powerlighttech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 06:09:03 2026 GMT\n  hsts: false\ndomains:\n- domain: powerlighttech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerlight-technologies/refs/heads/main/security/powerlight-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Wireless Power
- Power Beaming
- Lasers
- Aerospace
- Defense
- Space
- Telecom
- Hardware
---
