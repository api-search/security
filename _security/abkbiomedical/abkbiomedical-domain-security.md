---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: abkbiomedical.com
  spf: true
hosts:
- cert_expires: Oct 30 18:06:19 2026 GMT
  host: abkbiomedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abkbiomedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ABK Biomedical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ABK Biomedical
provider_slug: abkbiomedical
slug: abkbiomedical-domain-security
source_filename: abkbiomedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abkbiomedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 18:06:19 2026 GMT\n  hsts: false\ndomains:\n- domain: abkbiomedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abkbiomedical/refs/heads/main/security/abkbiomedical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical Devices
- Interventional Oncology
- Radioembolization
- Medical Imaging
- Oncology
- Healthcare
- Manufacturing
- Canada
- Company
---
