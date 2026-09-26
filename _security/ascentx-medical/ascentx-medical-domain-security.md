---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ascentxmedical.com
  spf: true
hosts:
- cert_expires: Nov 17 00:01:36 2026 GMT
  host: ascentxmedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ascentx Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AscentX Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AscentX Medical
provider_slug: ascentx-medical
slug: ascentx-medical-domain-security
source_filename: ascentx-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ascentxmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 00:01:36 2026 GMT\n  hsts: false\ndomains:\n- domain: ascentxmedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ascentx-medical/refs/heads/main/security/ascentx-medical-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Regenerative Medicine
- Tissue Engineering
- Healthcare
- Biotechnology
---
