---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: saksfifthavenue.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.saksfifthavenue.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saks Global Fka Saks Fifth Avenue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saks Global (fka Saks Fifth Avenue), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Saks Global (fka Saks Fifth Avenue)
provider_slug: saks-global-fka-saks-fifth-avenue
slug: saks-global-fka-saks-fifth-avenue-domain-security
source_filename: saks-global-fka-saks-fifth-avenue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saksfifthavenue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: saksfifthavenue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saks-global-fka-saks-fifth-avenue/refs/heads/main/security/saks-global-fka-saks-fifth-avenue-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- E-commerce
- Luxury
- Fashion
- Department Store
---
