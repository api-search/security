---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: arctherapeutics.com
  spf: false
hosts:
- cert_expires: Mar 21 09:58:52 2027 GMT
  host: www.arctherapeutics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arctherapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arctherapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Arctherapeutics
provider_slug: arctherapeutics
slug: arctherapeutics-domain-security
source_filename: arctherapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arctherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 09:58:52 2027 GMT\n  hsts: false\ndomains:\n- domain: arctherapeutics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arctherapeutics/refs/heads/main/security/arctherapeutics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Medical Devices
- Radiosurgery
- Oncology
---
