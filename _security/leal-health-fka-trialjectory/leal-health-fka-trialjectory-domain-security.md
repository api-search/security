---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leal.health
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: leal.health
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.leal.health
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: api.leal.health
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Leal Health Fka Trialjectory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leal Health (fka TrialJectory), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Leal Health (fka TrialJectory)
provider_slug: leal-health-fka-trialjectory
slug: leal-health-fka-trialjectory-domain-security
source_filename: leal-health-fka-trialjectory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leal.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: www.leal.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: api.leal.health\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: leal.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leal-health-fka-trialjectory/refs/heads/main/security/leal-health-fka-trialjectory-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Oncology
- Clinical Trials
- Patient Matching
- Artificial Intelligence
- Life Sciences
- Pharmaceuticals
- Decision Support
---
