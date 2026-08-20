---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paradromics.com
  spf: true
hosts:
- cert_expires: Sep  7 23:11:26 2026 GMT
  host: paradromics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paradromics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paradromics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paradromics
provider_slug: paradromics
slug: paradromics-domain-security
source_filename: paradromics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paradromics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:11:26 2026 GMT\n  hsts: false\ndomains:\n- domain: paradromics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradromics/refs/heads/main/security/paradromics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Brain-Computer Interface
- Neurotechnology
- Medical Devices
- Healthcare
- Implantable Devices
- Neural Data
- Assistive Technology
- Clinical Research
- Artificial Intelligence
---
