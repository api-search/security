---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: synapsor.com
  spf: true
hosts:
- cert_expires: Aug 16 23:59:59 2026 GMT
  host: synapsor.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Synapsor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synapsor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Synapsor
provider_slug: synapsor
slug: synapsor-domain-security
source_filename: synapsor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synapsor.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: synapsor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synapsor/refs/heads/main/security/synapsor-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Healthcare
- Medical Devices
- Wearables
- Continuous Glucose Monitoring
- Diabetes
- Internet of Things
---
