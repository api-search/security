---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: curb.com
  spf: true
hosts:
- cert_expires: Dec 16 15:17:49 2026 GMT
  host: www.curb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curb, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Curb
provider_slug: curb
slug: curb-domain-security
source_filename: curb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.curb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 15:17:49 2026 GMT\n  hsts: false\ndomains:\n- domain: curb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curb/refs/heads/main/security/curb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Entertainment
- Record Labels
- Media
---
