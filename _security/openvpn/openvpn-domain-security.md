---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openvpn.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openvpn.com
  spf: true
hosts:
- cert_expires: Feb  5 16:05:22 2027 GMT
  host: openvpn.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 20 16:52:02 2026 GMT
  host: myaccount.openvpn.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openvpn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenVPN, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenVPN
provider_slug: openvpn
slug: openvpn-domain-security
source_filename: openvpn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openvpn.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 16:05:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: myaccount.openvpn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 20 16:52:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: openvpn.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: openvpn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openvpn/refs/heads/main/security/openvpn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- VPN
- Zero Trust
- Network Security
- Remote Access
- Identity
- Cloud Security
---
