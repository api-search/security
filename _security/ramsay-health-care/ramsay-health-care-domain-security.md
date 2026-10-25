---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ramsayhealth.com
  spf: true
hosts:
- cert_expires: Dec  2 11:16:03 2026 GMT
  host: ramsayhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ramsay Health Care Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ramsay Health Care, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ramsay Health Care
provider_slug: ramsay-health-care
slug: ramsay-health-care-domain-security
source_filename: ramsay-health-care-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ramsayhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 11:16:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ramsayhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ramsay-health-care/refs/heads/main/security/ramsay-health-care-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Hospitals
- Private Healthcare
- Australia
- ASX Listed
---
