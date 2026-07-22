---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sanderson-farms.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: waynesandersonfarms.com
  spf: false
hosts:
- host: www.sanderson-farms.com
  https: false
- cert_expires: Sep 14 05:13:15 2026 GMT
  host: waynesandersonfarms.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sanderson Farms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sanderson Farms, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sanderson Farms
provider_slug: sanderson-farms
slug: sanderson-farms-domain-security
source_filename: sanderson-farms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sanderson-farms.com\n  https: false\n- host: waynesandersonfarms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:13:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sanderson-farms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: waynesandersonfarms.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanderson-farms/refs/heads/main/security/sanderson-farms-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Agriculture
- Food Production
- Fortune 1000
- Poultry
- Supply Chain
---
