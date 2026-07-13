---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ietf.org
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuemail "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:caa-reports@icann.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: iana.org
  spf: true
hosts:
- cert_expires: Oct  5 20:01:07 2026 GMT
  host: datatracker.ietf.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 21:37:55 2026 GMT
  host: www.iana.org
  hsts: true
  hsts_max_age: 48211200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snmp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SNMP, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SNMP
provider_slug: snmp
slug: snmp-domain-security
source_filename: snmp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datatracker.ietf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:01:07 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: www.iana.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:37:55 2026 GMT\n  hsts: true\n  hsts_max_age: 48211200\ndomains:\n- domain: ietf.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: iana.org\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuemail \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:caa-reports@icann.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snmp/refs/heads/main/security/snmp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SNMP
- Network Management
- Network Monitoring
- IETF
- Protocol
- MIB
- SMI
- OID
- Agents
- Traps
- UDP
- Operations
---
