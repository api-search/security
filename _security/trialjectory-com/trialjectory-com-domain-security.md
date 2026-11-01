---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trialjectory.com
  spf: true
hosts:
- cert_expires: Dec 30 02:16:44 2026 GMT
  host: www.trialjectory.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trialjectory Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leal Health (fka TrialJectory), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Leal Health (fka TrialJectory)
provider_slug: trialjectory-com
slug: trialjectory-com-domain-security
source_filename: trialjectory-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trialjectory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 02:16:44 2026 GMT\n  hsts: false\ndomains:\n- domain: trialjectory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/trialjectory-com/security/trialjectory-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cancer Treatment
- Decision Support
- Patient Support
---
