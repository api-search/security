---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ipulse-group.com
  spf: false
hosts:
- cert_expires: Nov  9 17:52:48 2026 GMT
  host: www.ipulse-group.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: I Pulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for I-Pulse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: I-Pulse
provider_slug: i-pulse
slug: i-pulse-domain-security
source_filename: i-pulse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ipulse-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 17:52:48 2026 GMT\n  hsts: false\ndomains:\n- domain: ipulse-group.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/i-pulse/refs/heads/main/security/i-pulse-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Industrial
- Energy
- Mining
- Manufacturing
- Semiconductors
- Geothermal
- Deep Tech
- Pulsed Power
---
