---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: layerhealth.com
  spf: true
hosts:
- cert_expires: Sep 30 17:24:37 2026 GMT
  host: www.layerhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Layer Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Layer Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Layer Health
provider_slug: layer-health
slug: layer-health-domain-security
source_filename: layer-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.layerhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:24:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: layerhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layer-health/refs/heads/main/security/layer-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Healthcare
- Artificial Intelligence
- Clinical Intelligence
- Electronic Health Records
- Digital Health
---
