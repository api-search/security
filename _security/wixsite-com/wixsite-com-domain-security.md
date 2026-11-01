---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wixsite.com
  spf: true
hosts:
- cert_expires: Dec 31 11:33:52 2026 GMT
  host: percolata.wixsite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wixsite Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Percolata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Percolata
provider_slug: wixsite-com
slug: wixsite-com-domain-security
source_filename: wixsite-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: percolata.wixsite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 11:33:52 2026 GMT\n  hsts: null\ndomains:\n- domain: wixsite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/wixsite-com/security/wixsite-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Analytics
- Retail
- Staffing
---
