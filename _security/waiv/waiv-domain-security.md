---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: waiv.com
  note: Current canonical web domain. No SPF or DMARC TXT record was returned on probe, while the legacy wearewaiv.com domain publishes both — the email posture has not followed the domain rename.
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wearewaiv.com
  spf: true
hosts:
- cert_expires: Oct 29 16:29:11 2026 GMT
  host: waiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:39:44 2026 GMT
  host: wearewaiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Legacy brand domain; 301 redirects to waiv.com. Still the published contact/mail domain (marketing@wearewaiv.com).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waiv, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Waiv
provider_slug: waiv
slug: waiv-domain-security
source_filename: waiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 16:29:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wearewaiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:39:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Legacy brand domain; 301 redirects to waiv.com. Still the published contact/mail\n    domain (marketing@wearewaiv.com).\ndomains:\n- domain: waiv.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: Current canonical web domain. No SPF or DMARC TXT record was returned on probe,\n    while the legacy wearewaiv.com domain publishes both — the email posture has not\n    followed the domain rename.\n- domain: wearewaiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waiv/refs/heads/main/security/waiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Data
- Artificial Intelligence
- Healthcare
- Digital Pathology
- Oncology
- Medical Diagnostics
- Precision Medicine
- Biomarkers
- Machine-Learning
- Life Sciences
- Medical Imaging
---
