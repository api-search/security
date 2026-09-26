---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appliedmedical.com
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: appliedmedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Applied Medical Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Applied Medical Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Applied Medical Resources
provider_slug: applied-medical-resources
slug: applied-medical-resources-domain-security
source_filename: applied-medical-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appliedmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: appliedmedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applied-medical-resources/refs/heads/main/security/applied-medical-resources-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical
- Devices
- Healthcare
- Surgery
---
