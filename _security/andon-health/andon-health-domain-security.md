---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ihealthlabs.com
  spf: true
hosts:
- cert_expires: Aug 30 19:14:02 2026 GMT
  host: ihealthlabs.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: developer.ihealthlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.ihealthlabs.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Andon Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andon Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Andon Health
provider_slug: andon-health
slug: andon-health-domain-security
source_filename: andon-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ihealthlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: developer.ihealthlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.ihealthlabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ihealthlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andon-health/refs/heads/main/security/andon-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medical Devices
- Digital Health
- Remote Patient Monitoring
- Connected Health
- IoT
- Wearables
---
