---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nference.com
  spf: true
hosts:
- cert_expires: Sep  1 21:05:06 2026 GMT
  host: nference.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nference Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nference, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: nference
provider_slug: nference
slug: nference-domain-security
source_filename: nference-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nference.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 21:05:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nference.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nference/refs/heads/main/security/nference-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthtech
- Artificial Intelligence
- Clinical Research
- Life Sciences
- Medical Imaging
- Data Science
- Biomarkers
---
