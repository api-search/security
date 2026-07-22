---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boringcompany.com
  spf: true
hosts:
- cert_expires: Oct 13 17:28:55 2026 GMT
  host: boringcompany.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Boring Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Boring Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Boring Company
provider_slug: the-boring-company
slug: the-boring-company-domain-security
source_filename: the-boring-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boringcompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:28:55 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: boringcompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-boring-company/refs/heads/main/security/the-boring-company-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Transportation
- Tunnels
- Transit
- Construction
- Loop
---
