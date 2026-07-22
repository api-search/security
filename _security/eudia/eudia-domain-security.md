---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eudia.com
  spf: true
hosts:
- cert_expires: Sep 12 02:32:31 2026 GMT
  host: eudia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eudia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eudia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eudia
provider_slug: eudia
slug: eudia-domain-security
source_filename: eudia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eudia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:32:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eudia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eudia/refs/heads/main/security/eudia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Legal Tech
- Artificial Intelligence
- Augmented Intelligence
- Compliance
- Contract Management
- Enterprise Software
---
