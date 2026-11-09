---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: applyall.com
  spf: true
hosts:
- cert_expires: Jan 12 13:15:45 2027 GMT
  host: applyall.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Applyall Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ApplyAll, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ApplyAll
provider_slug: applyall-com
slug: applyall-com-domain-security
source_filename: applyall-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: applyall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 13:15:45 2027 GMT\n  hsts: false\ndomains:\n- domain: applyall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/applyall-com/security/applyall-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Job Search
- Artificial Intelligence
- InterviewGuarantee
- Career Coaching
- White Label
---
