---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nociontx.com
  spf: true
hosts:
- cert_expires: Oct  2 05:09:45 2026 GMT
  host: nociontx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nocion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nocion Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nocion Therapeutics
provider_slug: nocion
slug: nocion-domain-security
source_filename: nocion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nociontx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:09:45 2026 GMT\n  hsts: false\ndomains:\n- domain: nociontx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nocion/refs/heads/main/security/nocion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biopharmaceutical
- Biotech
- Therapeutics
- Life Sciences
- Chronic Cough
- Drug Development
- Healthcare
---
