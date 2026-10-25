---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: promed.com.au
  spf: true
hosts:
- cert_expires: Dec 17 18:27:40 2026 GMT
  host: promed.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pro Medicus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pro Medicus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pro Medicus
provider_slug: pro-medicus
slug: pro-medicus-domain-security
source_filename: pro-medicus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promed.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 18:27:40 2026 GMT\n  hsts: false\ndomains:\n- domain: promed.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pro-medicus/refs/heads/main/security/pro-medicus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Imaging
- Radiology
- PACS
- RIS
- Health IT
- Australia
---
