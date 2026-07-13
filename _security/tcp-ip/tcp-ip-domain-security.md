---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ietf.org
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rfc-editor.org
  spf: true
hosts:
- cert_expires: Oct  5 20:01:07 2026 GMT
  host: www.ietf.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 05:02:36 2026 GMT
  host: www.rfc-editor.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tcp Ip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TCP/IP, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TCP/IP
provider_slug: tcp-ip
slug: tcp-ip-domain-security
source_filename: tcp-ip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ietf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:01:07 2026 GMT\n  hsts: false\n- host: www.rfc-editor.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:02:36 2026 GMT\n  hsts: false\ndomains:\n- domain: ietf.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rfc-editor.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tcp-ip/refs/heads/main/security/tcp-ip-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Networking
- Protocol
- Internet
- Standards
- IETF
- RFC
- TCP
- IP
---
