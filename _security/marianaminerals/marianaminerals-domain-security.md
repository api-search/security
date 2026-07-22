---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: marianaminerals.com
  spf: false
hosts:
- cert_expires: Oct 12 15:02:54 2026 GMT
  host: marianaminerals.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marianaminerals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marianaminerals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Marianaminerals
provider_slug: marianaminerals
slug: marianaminerals-domain-security
source_filename: marianaminerals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marianaminerals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 15:02:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marianaminerals.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marianaminerals/refs/heads/main/security/marianaminerals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Critical Minerals
- Mining
- Copper
- Lithium
- Energy
- Defense
- Supply Chain
---
