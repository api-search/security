---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: earlens.com
  spf: true
hosts:
- cert_expires: Sep 21 03:09:35 2026 GMT
  host: www.earlens.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Earlens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EarLens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EarLens
provider_slug: earlens
slug: earlens-domain-security
source_filename: earlens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.earlens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:09:35 2026 GMT\n  hsts: null\ndomains:\n- domain: earlens.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earlens/refs/heads/main/security/earlens-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hearing
- Hearing Aids
- Audiology
- Medical Devices
- Medical Technology
- Health
- Consumer Health
---
