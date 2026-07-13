---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: crossamericapartners.com
  spf: true
hosts:
- cert_expires: Sep  9 03:43:01 2026 GMT
  host: www.crossamericapartners.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.crossamericapartners.com
  https: false
- host: api.crossamericapartners.com
  https: false
kind: domain-security
layout: security
method: probed
name: Crossamerica Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrossAmerica Partners, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CrossAmerica Partners
provider_slug: crossamerica-partners
slug: crossamerica-partners-domain-security
source_filename: crossamerica-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crossamericapartners.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:43:01 2026 GMT\n  hsts: false\n- host: developer.crossamericapartners.com\n  https: false\n- host: api.crossamericapartners.com\n  https: false\ndomains:\n- domain: crossamericapartners.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossamerica-partners/refs/heads/main/security/crossamerica-partners-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fuel Distribution
- Convenience Stores
- Energy
---
