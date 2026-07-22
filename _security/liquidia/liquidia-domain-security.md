---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: liquidia.com
  spf: true
hosts:
- cert_expires: Oct 14 03:17:25 2026 GMT
  host: www.liquidia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liquidia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liquidia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Liquidia
provider_slug: liquidia
slug: liquidia-domain-security
source_filename: liquidia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liquidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 03:17:25 2026 GMT\n  hsts: null\ndomains:\n- domain: liquidia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquidia/refs/heads/main/security/liquidia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biopharmaceutical
- Pharmaceuticals
- Life Sciences
- Healthcare
- Drug Delivery
- Pulmonary Hypertension
- Clinical Trials
- Inhaled Therapeutics
---
