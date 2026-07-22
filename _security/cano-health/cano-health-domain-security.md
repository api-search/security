---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: canohealth.com
  spf: true
hosts:
- cert_expires: Aug 17 23:04:24 2026 GMT
  host: www.canohealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cano Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cano Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cano Health
provider_slug: cano-health
slug: cano-health-domain-security
source_filename: cano-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.canohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:04:24 2026 GMT\n  hsts: false\ndomains:\n- domain: canohealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cano-health/refs/heads/main/security/cano-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Primary Care
- Senior Care
- Value-Based Care
- Medical Centers
---
