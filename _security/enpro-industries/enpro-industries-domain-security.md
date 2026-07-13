---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enproindustries.com
  spf: true
hosts:
- cert_expires: Aug 26 11:35:40 2026 GMT
  host: www.enproindustries.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.enproindustries.com
  https: false
- host: api.enproindustries.com
  https: false
kind: domain-security
layout: security
method: probed
name: Enpro Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnPro Industries, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EnPro Industries
provider_slug: enpro-industries
slug: enpro-industries-domain-security
source_filename: enpro-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enproindustries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 11:35:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.enproindustries.com\n  https: false\n- host: api.enproindustries.com\n  https: false\ndomains:\n- domain: enproindustries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enpro-industries/refs/heads/main/security/enpro-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial
- Sealing
- Manufacturing
---
