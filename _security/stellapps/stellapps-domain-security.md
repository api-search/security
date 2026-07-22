---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stellapps.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: stellapps.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stellapps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stellapps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stellapps
provider_slug: stellapps
slug: stellapps-domain-security
source_filename: stellapps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stellapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: stellapps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellapps/refs/heads/main/security/stellapps-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Dairy
- Internet of Things
- Agriculture
- Supply Chain
- Cold Chain
- Herd Management
- Milk Procurement
- Machine Learning
- India
---
