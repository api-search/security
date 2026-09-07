---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: 4dbim.ren
  mx:
  - mxn.mxhichina.com
  - mxw.mxhichina.com
  registrar_dns: Alibaba Cloud (dns29/dns30.hichina.com)
  spf: false
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: 4dbim.cn
  mx: []
  registrar_dns: nowcndns.com (ns1/ns2)
  spf: false
hosts:
- cert_expires: null
  host: www.4dbim.ren
  hsts: false
  http: true
  https: false
  https_port_state: refused
  note: 'HTTP 200 at http://www.4dbim.ren/ which 302s to /zh. Port 443 refused: `nc -z www.4dbim.ren 443` fails and openssl s_client reports errno 61 (connection refused).'
  server: nginx
  tls_version: null
- cert_expires: null
  host: 4dbim.ren
  hsts: false
  http: true
  https: false
  https_port_state: refused
  note: Apex is an Aliyun URL-forwarding host that 302s every path to the matching path on www.4dbim.ren.
  server: Tengine (Aliyun URL Forwarding Server)
  tls_version: null
- cert_expires: null
  host: www.4dbim.cn
  hsts: false
  http: true
  https: false
  https_port_state: refused
  note: Secondary domain carried in the site footer contact address (market@4dbim.cn). It answers HTTP 404 at the root with an empty body and 403 with an empty body on every other path probed, including a random negative-control path — a blanket-deny host, not a document server. It publishes no MX record, so the footer address appears undeliverable; the contact page itself gives market@4dbim.ren.
  tls_version: null
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 4Dbim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4DBIM, probed live across 3 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 4DBIM
provider_slug: 4dbim
slug: 4dbim-domain-security
source_filename: 4dbim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TCP/TLS/HTTP probes of every host this record knows (www.4dbim.ren, 4dbim.ren, and\n  www.4dbim.cn, the domain used by the footer contact address). No OpenAPI servers[] host exists —\n  4DBIM publishes no machine-readable contract.\nnote: 'The primary web property is HTTP-only. TCP 443 on www.4dbim.ren is refused (connection refused,\n  not a timeout or a filtered drop), so there is no TLS to negotiate and no certificate to inspect; the\n  site is served over cleartext HTTP by nginx behind an Aliyun edge. 4dbim.ren also publishes no SPF,\n  no DMARC, no CAA and no DNSSEC. This is a domain-hygiene finding about the corporate web/mail\n  surface, not about an API — 4DBIM exposes no public API host.'\nhosts:\n- host: www.4dbim.ren\n  https: false\n  http: true\n  https_port_state: refused\n  tls_version: null\n  cert_expires: null\n  hsts: false\n  server: nginx\n  note: 'HTTP 200 at http://www.4dbim.ren/ which 302s to\
  \ /zh. Port 443 refused: `nc -z www.4dbim.ren 443`\n    fails and openssl s_client reports errno 61 (connection refused).'\n- host: 4dbim.ren\n  https: false\n  http: true\n  https_port_state: refused\n  tls_version: null\n  cert_expires: null\n  hsts: false\n  server: Tengine (Aliyun URL Forwarding Server)\n  note: Apex is an Aliyun URL-forwarding host that 302s every path to the matching path on www.4dbim.ren.\n- host: www.4dbim.cn\n  https: false\n  http: true\n  https_port_state: refused\n  tls_version: null\n  cert_expires: null\n  hsts: false\n  note: 'Secondary domain carried in the site footer contact address (market@4dbim.cn). It answers HTTP\n    404 at the root with an empty body and 403 with an empty body on every other path probed, including\n    a random negative-control path — a blanket-deny host, not a document server. It publishes no MX\n    record, so the footer address appears undeliverable; the contact page itself gives market@4dbim.ren.'\ndomains:\n- domain: 4dbim.ren\n\
  \  registrar_dns: Alibaba Cloud (dns29/dns30.hichina.com)\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  mx:\n  - mxn.mxhichina.com\n  - mxw.mxhichina.com\n- domain: 4dbim.cn\n  registrar_dns: nowcndns.com (ns1/ns2)\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  mx: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4dbim/refs/heads/main/security/4dbim-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Construction
- Construction Technology
- Building Information Modeling
- BIM
- Digital Twin
- Infrastructure
- Engineering
- Internet of Things
- SaaS
- China
---
