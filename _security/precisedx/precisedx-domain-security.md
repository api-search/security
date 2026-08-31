---
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: precisedx.ai
  spf: true
hosts:
- cert_expires: Oct 15 18:28:56 2026 GMT
  host: www.precisedx.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: portal.precisedx.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: Authenticated clinician ordering portal (PDx Portal / Order Portal). Added by hand from a live TLS/HTTP probe on 2026-08-26 because probe-domain-security.py reads baseURL/servers[] hosts and this host is only referenced from the Login pointer.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Precisedx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PreciseDx, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: PreciseDx
provider_slug: precisedx
slug: precisedx-domain-security
source_filename: precisedx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.precisedx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:28:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.precisedx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: >-\n    Authenticated clinician ordering portal (PDx Portal / Order Portal). Added by hand\n    from a live TLS/HTTP probe on 2026-08-26 because probe-domain-security.py reads\n    baseURL/servers[] hosts and this host is only referenced from the Login pointer.\ndomains:\n- domain: precisedx.ai\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/precisedx/refs/heads/main/security/precisedx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Digital Pathology
- Oncology
- Artificial Intelligence
- Machine-Learning
- Clinical Laboratory
- Precision Medicine
---
