---
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issue "sectigo.com"
  - 128 issue "amazon.com"
  - 128 issue "ZScaler.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: juniper.net
  spf: true
- caa:
  - 128 issue "google.com"
  - 128 issue "Godaddy.com"
  - 128 issue "sectigo.com"
  - 128 issue "amazon.com"
  - 128 issue "digicert.com"
  - 128 issue "ZScaler.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 128technology.com
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: www.juniper.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 18:03:19 2026 GMT
  host: docs.128technology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 128 Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 128 Technology, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 128 Technology
provider_slug: 128-technology
slug: 128-technology-domain-security
source_filename: 128-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.juniper.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.128technology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 18:03:19 2026 GMT\n  hsts: false\ndomains:\n- domain: juniper.net\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"sectigo.com\"\n  - 128 issue \"amazon.com\"\n  - 128 issue \"ZScaler.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: 128technology.com\n  dnssec: false\n  caa:\n  - 128 issue \"google.com\"\n  - 128 issue \"Godaddy.com\"\n  - 128 issue \"sectigo.com\"\n  - 128 issue \"amazon.com\"\n  - 128 issue \"digicert.com\"\n  - 128 issue \"ZScaler.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/128-technology/refs/heads/main/security/128-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Networking
- SD-WAN
- Routing
- Network Management
- Session Smart Networking
- NETCONF
- YANG
- Telecommunications
- Infrastructure
---
