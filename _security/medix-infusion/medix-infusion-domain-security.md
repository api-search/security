---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medixinfusion.com
  spf: true
hosts:
- cert_expires: Oct  2 20:49:13 2026 GMT
  host: medixinfusion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medix Infusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medix Infusion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Medix Infusion
provider_slug: medix-infusion
slug: medix-infusion-domain-security
source_filename: medix-infusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medixinfusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:49:13 2026 GMT\n  hsts: false\ndomains:\n- domain: medixinfusion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medix-infusion/refs/heads/main/security/medix-infusion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Infusion Therapy
- Specialty Pharmacy
- Home Health
- Ambulatory Care
- Patient Care
- Texas
---
