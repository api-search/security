---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cerevasc.com
  spf: true
hosts:
- cert_expires: Oct 21 18:24:40 2026 GMT
  host: cerevasc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cerevasc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CereVasc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CereVasc
provider_slug: cerevasc
slug: cerevasc-domain-security
source_filename: cerevasc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cerevasc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 18:24:40 2026 GMT\n  hsts: false\ndomains:\n- domain: cerevasc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerevasc/refs/heads/main/security/cerevasc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Neurology
- Hydrocephalus
- Medical Technology
- Clinical Stage
---
