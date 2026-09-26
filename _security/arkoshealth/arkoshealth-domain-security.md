---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arkoshealth.com
  spf: true
hosts:
- cert_expires: Dec 16 04:57:21 2026 GMT
  host: arkoshealth.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arkoshealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arkoshealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Arkoshealth
provider_slug: arkoshealth
slug: arkoshealth-domain-security
source_filename: arkoshealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arkoshealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 16 04:57:21 2026 GMT\n  hsts: false\ndomains:\n- domain: arkoshealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arkoshealth/refs/heads/main/security/arkoshealth-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Healthcare
- Technology
- Value-based Care
- Platform
---
