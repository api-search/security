---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cabelas.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.cabelas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cabelas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cabela''s, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cabela's
provider_slug: cabelas
slug: cabelas-domain-security
source_filename: cabelas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cabelas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cabelas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cabelas/refs/heads/main/security/cabelas-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail
- Outdoor
- Hunting
- Fishing
- Camping
- E-Commerce
- Company
- Fortune 1000
---
