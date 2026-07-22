---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: andaafrica.com
  spf: true
hosts:
- cert_expires: Sep  6 09:27:15 2026 GMT
  host: andaafrica.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anda
provider_slug: anda
slug: anda-domain-security
source_filename: anda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: andaafrica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:27:15 2026 GMT\n  hsts: false\ndomains:\n- domain: andaafrica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anda/refs/heads/main/security/anda-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mobility
- Ride-hailing
- Delivery
- Transportation
- Fintech
- Electric Vehicles
- Sustainability
- Africa
- Angola
---
