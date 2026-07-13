---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: whatnot.com
  spf: true
hosts:
- cert_expires: Oct  6 12:50:23 2026 GMT
  host: www.whatnot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whatnot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whatnot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Whatnot
provider_slug: whatnot
slug: whatnot-domain-security
source_filename: whatnot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.whatnot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:50:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whatnot.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whatnot/refs/heads/main/security/whatnot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Marketplace
- Live Commerce
- Collectibles
- Resale
---
