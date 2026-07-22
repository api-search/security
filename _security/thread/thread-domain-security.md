---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thread.com
  spf: true
hosts:
- cert_expires: Sep 22 13:53:22 2026 GMT
  host: www.thread.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thread Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thread, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Thread
provider_slug: thread
slug: thread-domain-security
source_filename: thread-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thread.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:53:22 2026 GMT\n  hsts: false\ndomains:\n- domain: thread.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thread/refs/heads/main/security/thread-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fashion
- Retail
- Styling
- Artificial Intelligence
- E-Commerce
- Defunct
---
