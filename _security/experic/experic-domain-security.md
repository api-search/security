---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: expericservices.com
  spf: true
hosts:
- cert_expires: Oct 10 15:02:18 2026 GMT
  host: expericservices.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Experic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Experic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Experic
provider_slug: experic
slug: experic-domain-security
source_filename: experic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: expericservices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 15:02:18 2026 GMT\n  hsts: false\ndomains:\n- domain: expericservices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/experic/refs/heads/main/security/experic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Life Sciences
- Manufacturing
- CDMO
- Clinical Trials
- Contract Manufacturing
- Drug Delivery
- Supply Chain
- Packaging
---
