---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arlp.com
  spf: true
hosts:
- cert_expires: Sep 27 10:22:36 2026 GMT
  host: www.arlp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.arlp.com
  https: false
- host: api.arlp.com
  https: false
kind: domain-security
layout: security
method: probed
name: Alliance Resource Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alliance Resource Partners, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alliance Resource Partners
provider_slug: alliance-resource-partners
slug: alliance-resource-partners-domain-security
source_filename: alliance-resource-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arlp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:22:36 2026 GMT\n  hsts: false\n- host: developer.arlp.com\n  https: false\n- host: api.arlp.com\n  https: false\ndomains:\n- domain: arlp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alliance-resource-partners/refs/heads/main/security/alliance-resource-partners-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Coal
- Mining
- Energy
---
