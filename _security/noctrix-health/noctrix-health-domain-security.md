---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: noctrixhealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nidrarls.com
  spf: true
hosts:
- cert_expires: Oct 19 16:48:24 2026 GMT
  host: noctrixhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 19:09:10 2026 GMT
  host: nidrarls.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noctrix Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noctrix Health, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Noctrix Health
provider_slug: noctrix-health
slug: noctrix-health-domain-security
source_filename: noctrix-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noctrixhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 16:48:24 2026 GMT\n  hsts: false\n- host: nidrarls.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 19:09:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: noctrixhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nidrarls.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noctrix-health/refs/heads/main/security/noctrix-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Medical Devices
- Digital Health
- Sleep
- Neurology
- Neurostimulation
- Wearables
- MCP
- Agent Readiness
---
