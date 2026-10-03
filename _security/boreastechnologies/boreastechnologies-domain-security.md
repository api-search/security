---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boreas.ca
  spf: true
hosts:
- cert_expires: Dec  3 16:54:32 2026 GMT
  host: www.boreas.ca
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boreastechnologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boréastechnologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Boréastechnologies
provider_slug: boreastechnologies
slug: boreastechnologies-domain-security
source_filename: boreastechnologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boreas.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:54:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: boreas.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boreastechnologies/refs/heads/main/security/boreastechnologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Haptics
- Piezoelectric
- IoT
- Automotive
---
