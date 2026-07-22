---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shinehe.com
  spf: true
hosts:
- cert_expires: Dec  1 03:35:03 2026 GMT
  host: www.shinehe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shinehe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shinehe (Hangzhou Xinzeyuan Medical Technology), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Shinehe (Hangzhou Xinzeyuan Medical Technology)
provider_slug: shinehe
slug: shinehe-domain-security
source_filename: shinehe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shinehe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 03:35:03 2026 GMT\n  hsts: false\ndomains:\n- domain: shinehe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shinehe/refs/heads/main/security/shinehe-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Medical Devices
- Healthcare
- CDMO
- Manufacturing
- Minimally Invasive Surgery
- Endoscopy
- China
---
