---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acera-surgical.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: acera-surgical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acerasurgical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acera Surgical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acera Surgical
provider_slug: acerasurgical
slug: acerasurgical-domain-security
source_filename: acerasurgical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acera-surgical.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acera-surgical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acerasurgical/refs/heads/main/security/acerasurgical-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Regenerative Medicine
- Wound Care
- Biotechnology
- Surgical
- Life Sciences
- Healthcare
---
