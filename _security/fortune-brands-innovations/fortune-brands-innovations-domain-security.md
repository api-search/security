---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fbin.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.fbin.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: developer.fbin.com
  https: false
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: api.fbin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fortune Brands Innovations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortune Brands Innovations, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Fortune Brands Innovations
provider_slug: fortune-brands-innovations
slug: fortune-brands-innovations-domain-security
source_filename: fortune-brands-innovations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fbin.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\n- host: developer.fbin.com\n  https: false\n- host: api.fbin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fbin.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortune-brands-innovations/refs/heads/main/security/fortune-brands-innovations-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Home Products
- Hardware
- Security
- Fortune 1000
---
