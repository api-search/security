---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: huronconsultinggroup.com
  spf: true
hosts:
- cert_expires: Aug 12 00:39:00 2026 GMT
  host: www.huronconsultinggroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.huronconsultinggroup.com
  https: false
- host: api.huronconsultinggroup.com
  https: false
kind: domain-security
layout: security
method: probed
name: Huron Consulting Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huron Consulting Group, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Huron Consulting Group
provider_slug: huron-consulting-group
slug: huron-consulting-group-domain-security
source_filename: huron-consulting-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.huronconsultinggroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 00:39:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.huronconsultinggroup.com\n  https: false\n- host: api.huronconsultinggroup.com\n  https: false\ndomains:\n- domain: huronconsultinggroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huron-consulting-group/refs/heads/main/security/huron-consulting-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consulting
- Healthcare
- Education
---
