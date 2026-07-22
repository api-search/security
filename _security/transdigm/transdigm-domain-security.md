---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transdigm.com
  spf: true
hosts:
- cert_expires: Aug 20 17:39:32 2026 GMT
  host: www.transdigm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transdigm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TransDigm Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TransDigm Group
provider_slug: transdigm
slug: transdigm-domain-security
source_filename: transdigm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transdigm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:39:32 2026 GMT\n  hsts: false\ndomains:\n- domain: transdigm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transdigm/refs/heads/main/security/transdigm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aerospace
- Defense
- Manufacturing
- Fortune 500
- Proprietary Components
---
