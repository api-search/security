---
description: ''
domains:
- caa:
  - 128 iodef "mailto:infosec@cisco.com"
  - 0 issue "digicert.com"
  - 128 issuewild "digicert.com"
  - 0 issue "ssl.com"
  - 128 issuewild "ssl.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cisco.com
  spf: true
hosts:
- cert_expires: Feb 20 00:05:07 2027 GMT
  host: developer.cisco.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Aci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco ACI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco ACI
provider_slug: cisco-aci
slug: cisco-aci-domain-security
source_filename: cisco-aci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 0 issue \"digicert.com\"\n  - 128 issuewild \"digicert.com\"\n  - 0 issue \"ssl.com\"\n  - 128 issuewild \"ssl.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-aci/refs/heads/main/security/cisco-aci-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SDN
- Data Center
- Networking
- Fabric
- Automation
- Enterprise
- Network Automation
- Infrastructure
- Controller
- REST API
---
