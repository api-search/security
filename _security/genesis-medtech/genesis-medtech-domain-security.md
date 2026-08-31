---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: genesismedtech.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.genesismedtech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genesis Medtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genesis Medtech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Genesis Medtech
provider_slug: genesis-medtech
slug: genesis-medtech-domain-security
source_filename: genesis-medtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genesismedtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: genesismedtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genesis-medtech/refs/heads/main/security/genesis-medtech-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Medical Devices
- Surgical
- Structural Heart
- Vascular Intervention
- Medtech
---
