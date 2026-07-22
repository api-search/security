---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pyxusinternational.com
  spf: true
hosts:
- cert_expires: Aug 24 18:19:20 2026 GMT
  host: www.pyxusinternational.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alliance One International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for alliance-one-international, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: alliance-one-international
provider_slug: alliance-one-international
slug: alliance-one-international-domain-security
source_filename: alliance-one-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pyxusinternational.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:19:20 2026 GMT\n  hsts: false\ndomains:\n- domain: pyxusinternational.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alliance-one-international/refs/heads/main/security/alliance-one-international-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Tobacco
- Agriculture
- Commodities
- Leaf Tobacco
- Manufacturing
---
