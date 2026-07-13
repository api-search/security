---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anixter.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wesco.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.anixter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 18:26:28 2026 GMT
  host: www.wesco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anixter International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anixter International, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anixter International
provider_slug: anixter-international
slug: anixter-international-domain-security
source_filename: anixter-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anixter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\n- host: www.wesco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:26:28 2026 GMT\n  hsts: null\ndomains:\n- domain: anixter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wesco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anixter-international/refs/heads/main/security/anixter-international-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- B2B Commerce
- Cables
- Data Communications
- Distribution
- Electrical
- Industrial
- Network Infrastructure
- Security Solutions
- Supply Chain
- Wesco
- Fortune 500
---
