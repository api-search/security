---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nuvolo.com
  spf: true
hosts:
- cert_expires: Aug 22 23:14:14 2026 GMT
  host: www.nuvolo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuvolo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuvolo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nuvolo
provider_slug: nuvolo
slug: nuvolo-domain-security
source_filename: nuvolo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nuvolo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:14:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nuvolo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuvolo/refs/heads/main/security/nuvolo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IWMS
- Enterprise Asset Management
- Facilities Management
- Connected Workplace
- Healthcare Technology Management
- Space Management
- Real Estate
- Maintenance Management
- ServiceNow
- OT Security
- Sustainability
---
