---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: orapharma.com
  spf: true
hosts:
- cert_expires: Sep  9 07:29:28 2026 GMT
  host: www.orapharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orapharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orapharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Orapharma
provider_slug: orapharma
slug: orapharma-domain-security
source_filename: orapharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orapharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:29:28 2026 GMT\n  hsts: false\ndomains:\n- domain: orapharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orapharma/refs/heads/main/security/orapharma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Oral Health
- Dental
- Periodontics
- Healthcare
- Life Sciences
---
