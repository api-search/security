---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: binsentry.com
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: www.binsentry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Binsentry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binsentry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Binsentry
provider_slug: binsentry
slug: binsentry-domain-security
source_filename: binsentry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.binsentry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: binsentry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binsentry/refs/heads/main/security/binsentry-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- FeedManagement
- Agriculture
- IoT
- Inventory
---
