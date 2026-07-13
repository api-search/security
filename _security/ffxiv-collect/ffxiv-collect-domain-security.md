---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ffxivcollect.com
  spf: true
hosts:
- cert_expires: Aug 23 14:59:33 2026 GMT
  host: ffxivcollect.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ffxiv Collect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FFXIV Collect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FFXIV Collect
provider_slug: ffxiv-collect
slug: ffxiv-collect-domain-security
source_filename: ffxiv-collect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ffxivcollect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 14:59:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ffxivcollect.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ffxiv-collect/refs/heads/main/security/ffxiv-collect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Games And Comics
- Public APIs
---
