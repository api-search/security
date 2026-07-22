---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tri-apex.com
  spf: true
hosts:
- cert_expires: Sep  1 04:27:24 2026 GMT
  host: www.tri-apex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tripod Glp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tripod-glp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: tripod-glp
provider_slug: tripod-glp
slug: tripod-glp-domain-security
source_filename: tripod-glp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tri-apex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:27:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tri-apex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripod-glp/refs/heads/main/security/tripod-glp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Contract Research Organization
- Pharmaceutical
- Biomedical Research
- Clinical Trials
- Preclinical
- Life Sciences
- Healthcare
---
