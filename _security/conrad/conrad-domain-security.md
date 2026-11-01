---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conrad.com
  spf: true
hosts:
- cert_expires: Dec 10 04:16:14 2026 GMT
  host: www.conrad.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Conrad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conrad Electronic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Conrad Electronic
provider_slug: conrad
slug: conrad-domain-security
source_filename: conrad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conrad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 04:16:14 2026 GMT\n  hsts: null\ndomains:\n- domain: conrad.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/conrad/security/conrad-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Electronics
- Retail
- E-commerce
- DIY
---
