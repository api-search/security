---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: supiramedical.com
  spf: true
hosts:
- cert_expires: Oct  1 04:00:54 2026 GMT
  host: supiramedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Supira Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Supira Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Supira Medical
provider_slug: supira-medical
slug: supira-medical-domain-security
source_filename: supira-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  Probed 2026-08-29. TLS 1.3 with a valid certificate, but no HSTS, no CAA record, and no\n  DNSSEC. SPF is published. DMARC is NOT enforced: a `v=DMARC1;p=none;...` string is\n  published as an apex TXT record on supiramedical.com instead of at _dmarc.supiramedical.com,\n  and _dmarc.supiramedical.com returns no TXT record, so no receiver will apply the policy.\n  The web origin sits behind a SiteGround bot-challenge (HTTP 202, `sg-captcha: challenge`)\n  which answered every path probed.\nhosts:\n- host: supiramedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:00:54 2026 GMT\n  hsts: false\ndomains:\n- domain: supiramedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supira-medical/refs/heads/main/security/supira-medical-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Medical Devices
- Healthcare
- Cardiovascular
- Heart Pump
- Clinical Stage
- Medical Technology
- Private Company
---
