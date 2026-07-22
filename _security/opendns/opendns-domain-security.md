---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "identrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "quovadisglobal.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opendns.com
  spf: true
hosts:
- cert_expires: Oct  3 22:55:09 2026 GMT
  host: www.opendns.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Opendns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenDNS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenDNS
provider_slug: opendns
slug: opendns-domain-security
source_filename: opendns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opendns.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 22:55:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: opendns.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendns/refs/heads/main/security/opendns-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- DNS
- Security
- Content Filtering
- Threat Intelligence
- Networking
- Cisco
---
