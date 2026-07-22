---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fbin.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fortunebrands.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.fbin.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: www.fortunebrands.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fortune Brands Home And Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortune Brands Innovations, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Fortune Brands Innovations
provider_slug: fortune-brands-home-and-security
slug: fortune-brands-home-and-security-domain-security
source_filename: fortune-brands-home-and-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fbin.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\n- host: www.fortunebrands.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fbin.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: fortunebrands.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortune-brands-home-and-security/refs/heads/main/security/fortune-brands-home-and-security-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Fortune 500
- Home Products
- Water
- Security
- Outdoors
---
