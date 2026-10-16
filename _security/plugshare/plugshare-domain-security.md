---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plugshare.com
  spf: true
hosts:
- cert_expires: Jan 11 02:21:37 2027 GMT
  host: www.plugshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Plugshare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlugShare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PlugShare
provider_slug: plugshare
slug: plugshare-domain-security
source_filename: plugshare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plugshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 02:21:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plugshare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plugshare/refs/heads/main/security/plugshare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
