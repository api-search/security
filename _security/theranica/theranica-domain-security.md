---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theranica.com
  spf: true
hosts:
- cert_expires: Oct  3 08:23:48 2026 GMT
  host: theranica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Theranica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Theranica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Theranica
provider_slug: theranica
slug: theranica-domain-security
source_filename: theranica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theranica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:23:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: theranica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theranica/refs/heads/main/security/theranica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Therapeutics
- Medical Devices
- Neuromodulation
- Migraine
- Healthcare
- Wearables
- Bioelectronics
---
