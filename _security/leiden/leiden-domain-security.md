---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: universiteitleiden.nl
  spf: true
hosts:
- cert_expires: Aug 18 15:20:10 2026 GMT
  host: www.universiteitleiden.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 08:58:00 2026 GMT
  host: scholarlypublications.universiteitleiden.nl
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leiden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leiden University, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Leiden University
provider_slug: leiden
slug: leiden-domain-security
source_filename: leiden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.universiteitleiden.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 15:20:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: scholarlypublications.universiteitleiden.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 08:58:00 2026 GMT\n  hsts: false\ndomains:\n- domain: universiteitleiden.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leiden/refs/heads/main/security/leiden-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Netherlands
- Library
- Open Access
- OAI-PMH
- Research
---
