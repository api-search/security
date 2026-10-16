---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clearflow.com
  spf: true
hosts:
- cert_expires: Dec 31 20:12:31 2026 GMT
  host: clearflow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clearflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClearFlow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClearFlow
provider_slug: clearflow
slug: clearflow-domain-security
source_filename: clearflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clearflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 20:12:31 2026 GMT\n  hsts: false\ndomains:\n- domain: clearflow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearflow/refs/heads/main/security/clearflow-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical Devices
- Surgery
- Healthcare
- Innovation
- Patient Recovery
---
