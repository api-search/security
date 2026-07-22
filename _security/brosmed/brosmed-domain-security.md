---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brosmed.com
  spf: true
hosts:
- cert_expires: Dec 12 12:00:00 2026 GMT
  host: www.brosmed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brosmed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brosmed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Brosmed
provider_slug: brosmed
slug: brosmed-domain-security
source_filename: brosmed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brosmed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 12:00:00 2026 GMT\n  hsts: false\ndomains:\n- domain: brosmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brosmed/refs/heads/main/security/brosmed-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Medical Devices
- Medical Technology
- Cardiovascular
- Vascular Intervention
- China
---
