---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scopely.com
  spf: true
hosts:
- cert_expires: Aug 23 06:08:53 2026 GMT
  host: www.scopely.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scopely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scopely, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scopely
provider_slug: scopely
slug: scopely-domain-security
source_filename: scopely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scopely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:08:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: scopely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scopely/refs/heads/main/security/scopely-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Mobile Games
- Video Games
- Interactive Entertainment
- Game Publishing
- Live Operations
---
