---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kytentech.com
  spf: true
hosts:
- cert_expires: Sep 30 01:17:17 2026 GMT
  host: kytentech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kyten Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kyten Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kyten Technologies
provider_slug: kyten-technologies
slug: kyten-technologies-domain-security
source_filename: kyten-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kytentech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:17:17 2026 GMT\n  hsts: null\ndomains:\n- domain: kytentech.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyten-technologies/refs/heads/main/security/kyten-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hardware
- Manufacturing
- Aerospace
- Batteries
- Energy Storage
- Robotics
- Industrials
- Drones
- Satellites
---
