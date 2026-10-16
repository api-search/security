---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chimneytrailhealth.com
  spf: true
hosts:
- cert_expires: Jan  3 09:02:52 2027 GMT
  host: www.chimneytrailhealth.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chimney Trail Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chimney Trail Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chimney Trail Health
provider_slug: chimney-trail-health
slug: chimney-trail-health-domain-security
source_filename: chimney-trail-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chimneytrailhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 09:02:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: chimneytrailhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chimney-trail-health/refs/heads/main/security/chimney-trail-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MentalHealth
- Training
- Military
- Corporate
- Resilience
---
