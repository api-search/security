---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:itsecmon@expandenergy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chk.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.chk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chesapeake Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chesapeake Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chesapeake Energy
provider_slug: chesapeake-energy
slug: chesapeake-energy-domain-security
source_filename: chesapeake-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: chk.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:itsecmon@expandenergy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chesapeake-energy/refs/heads/main/security/chesapeake-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Expand Energy
- Exploration
- Marcellus
- Natural Gas
- Natural Gas Liquids
- Oil
- Oklahoma City
- Production
- Unconventional
- Fortune 500
---
