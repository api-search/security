---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hearst.com
  spf: true
hosts:
- cert_expires: Aug  4 07:53:09 2026 GMT
  host: www.hearst.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hearst Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hearst, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hearst
provider_slug: hearst-corporation
slug: hearst-corporation-domain-security
source_filename: hearst-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hearst.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 07:53:09 2026 GMT\n  hsts: null\ndomains:\n- domain: hearst.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hearst-corporation/refs/heads/main/security/hearst-corporation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Media
- Publishing
- Broadcasting
- Magazines
- Newspapers
- Television
- Cable Networks
- Healthcare Information
- Financial Information
- Automotive Data
- Syndication
- Conglomerate
- Private
---
