---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: celerion.com
  spf: true
hosts:
- cert_expires: Oct  8 17:30:41 2026 GMT
  host: www.celerion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Celerion Hig Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celerion (H.I.G. Capital), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Celerion (H.I.G. Capital)
provider_slug: celerion-hig-capital
slug: celerion-hig-capital-domain-security
source_filename: celerion-hig-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.celerion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:30:41 2026 GMT\n  hsts: false\ndomains:\n- domain: celerion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celerion-hig-capital/refs/heads/main/security/celerion-hig-capital-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Clinical Research
- Contract Research Organization
- Drug Development
- Bioanalytical Services
- Clinical Pharmacology
- Life Sciences
---
