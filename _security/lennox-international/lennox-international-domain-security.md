---
description: ''
domains:
- caa:
  - 128 issue "digicert.com"
  - 128 issuewild "entrust.net"
  - 128 issue "entrust.net"
  - 128 issuewild "sectigo.com"
  - 128 issue "sectigo.com"
  - 128 iodef "mailto:DISTLIST_ITOps_Windows_Server@LennoxInd.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lennox.com
  spf: true
- caa:
  - 128 issue "entrust.net"
  - 128 issuewild "sectigo.com"
  - 128 issue "sectigo.com"
  - 128 issue "digicert.com"
  - 128 iodef "mailto:DISTLIST_ITOps_Windows_Server@LennoxInd.com"
  - 128 issuewild "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lennoxinternational.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.lennox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: www.lennoxinternational.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.lennoxpros.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lennox International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lennox International, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lennox International
provider_slug: lennox-international
slug: lennox-international-domain-security
source_filename: lennox-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lennox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.lennoxinternational.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.lennoxpros.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lennox.com\n  dnssec: false\n  caa:\n  - 128 issue \"digicert.com\"\n  - 128 issuewild \"entrust.net\"\n  - 128 issue \"entrust.net\"\n  - 128 issuewild \"sectigo.com\"\n  - 128 issue \"sectigo.com\"\n  - 128 iodef \"mailto:DISTLIST_ITOps_Windows_Server@LennoxInd.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lennoxinternational.com\n  dnssec: false\n  caa:\n  - 128 issue \"entrust.net\"\n  - 128 issuewild\
  \ \"sectigo.com\"\n  - 128 issue \"sectigo.com\"\n  - 128 issue \"digicert.com\"\n  - 128 iodef \"mailto:DISTLIST_ITOps_Windows_Server@LennoxInd.com\"\n  - 128 issuewild \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lennox-international/refs/heads/main/security/lennox-international-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HVAC
- Smart Home
- Thermostat
- IoT
- Climate Control
- Fortune 1000
---
