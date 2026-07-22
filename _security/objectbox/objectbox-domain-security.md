---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=90; sp=none
  dnssec: false
  domain: objectbox.io
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- host: objectbox.io
  hsts: false
  hsts_max_age: null
  https: true
  server: Apache
kind: domain-security
layout: security
method: probed
name: Objectbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ObjectBox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ObjectBox
provider_slug: objectbox
slug: objectbox-domain-security
source_filename: objectbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live TLS/HTTP HEAD + dig against objectbox.io\nhosts:\n  - host: objectbox.io\n    https: true\n    server: Apache\n    hsts: false\n    hsts_max_age: null\ndomains:\n  - domain: objectbox.io\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: 'v=spf1 include:_spf.google.com ~all'\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_record: 'v=DMARC1; p=quarantine; pct=90; sp=none'\nnotes: >-\n  HTTPS reachable (Apache origin); no HSTS response header observed. No DNSSEC (no\n  DS record) and no CAA records published. SPF and DMARC are configured (DMARC at\n  p=quarantine, pct=90, subdomain policy none). Absence of HSTS/DNSSEC/CAA is\n  recorded as valid probe data, not fabricated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/objectbox/refs/heads/main/security/objectbox-domain-security.yml
summary_line: DMARC
tags:
- Company
- Database
- Embedded Database
- Mobile Database
- Edge Computing
- Vector Database
- Vector Search
- Offline First
- Data Sync
- Edge AI
- IoT
---
