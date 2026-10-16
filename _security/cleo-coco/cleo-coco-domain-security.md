---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cleoandcoco.com
  spf: true
hosts:
- cert_expires: Dec 25 23:36:31 2026 GMT
  host: cleoandcoco.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cleo Coco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cleo+Coco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cleo+Coco
provider_slug: cleo-coco
slug: cleo-coco-domain-security
source_filename: cleo-coco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cleoandcoco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:36:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: cleoandcoco.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleo-coco/refs/heads/main/security/cleo-coco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Deodorant
- Personal Care
- Body Powder
- Functional Spray
- Clean Beauty
---
