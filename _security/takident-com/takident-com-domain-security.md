---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    agents: []
    checked: '2026-11-26'
    index:
    - alpn:
      - h2
      target: www.takident.com
    published: true
  dnssec: true
  domain: takident.com
  spf: true
hosts:
- cert_expires: Feb 21 16:54:33 2027 GMT
  host: takident.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taki Dent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taki Dent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Taki Dent
provider_slug: takident-com
slug: takident-com-domain-security
source_filename: takident-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: takident.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 16:54:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: takident.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: true\n    index:\n    - target: www.takident.com\n      alpn:\n      - h2\n    agents: []\n"
source_yaml_url: https://artifacts.apis.io/takident-com/security/takident-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Dental
- Healthcare
- Clinic
- Turkey
- Cosmetic
---
