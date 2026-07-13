---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: darpa.mil
  spf: true
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.darpa.mil
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defense Advanced Research Projects Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Advanced Research Projects Agency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Defense Advanced Research Projects Agency
provider_slug: defense-advanced-research-projects-agency
slug: defense-advanced-research-projects-agency-domain-security
source_filename: defense-advanced-research-projects-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.darpa.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: darpa.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-advanced-research-projects-agency/refs/heads/main/security/defense-advanced-research-projects-agency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Defense
- Research
- Department of Defense
- DARPA
- Innovation
---
