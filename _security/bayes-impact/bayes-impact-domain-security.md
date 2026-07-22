---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bayesimpact.org
  spf: true
hosts:
- cert_expires: Sep 30 21:11:28 2026 GMT
  host: www.bayesimpact.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bayes Impact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bayes Impact, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Bayes Impact
provider_slug: bayes-impact
slug: bayes-impact-domain-security
source_filename: bayes-impact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bayesimpact.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:11:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bayesimpact.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bayes-impact/refs/heads/main/security/bayes-impact-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Nonprofit
- Artificial Intelligence
- Data Science
- Public Services
- Civic Tech
- Employment
- Open Source
- Protobuf
---
