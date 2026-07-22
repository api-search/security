---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lyondellbasell.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: www.lyondellbasell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lyondellbasell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LyondellBasell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LyondellBasell
provider_slug: lyondellbasell
slug: lyondellbasell-domain-security
source_filename: lyondellbasell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lyondellbasell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lyondellbasell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lyondellbasell/refs/heads/main/security/lyondellbasell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Petrochemicals
- Polymers
- Polyolefins
- Polyethylene
- Polypropylene
- Chemicals
- Plastics
- Refining
- Industrial
- Sustainability
- Recycled Plastics
- No APIs
---
