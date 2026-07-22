---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: xwork.co
  spf: true
hosts:
- cert_expires: Aug 31 04:58:52 2026 GMT
  host: xwork.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xwork, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Xwork
provider_slug: xwork
slug: xwork-domain-security
source_filename: xwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xwork.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:58:52 2026 GMT\n  hsts: false\ndomains:\n- domain: xwork.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xwork/refs/heads/main/security/xwork-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
---
