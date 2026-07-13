---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: harvard.edu
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: harvardartmuseums.org
  spf: false
hosts:
- cert_expires: Oct  8 05:40:58 2026 GMT
  host: www.harvard.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:45:57 2026 GMT
  host: api.harvardartmuseums.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:07:23 2026 GMT
  host: library.harvard.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harvard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harvard University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Harvard University
provider_slug: harvard
slug: harvard-domain-security
source_filename: harvard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.harvard.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:40:58 2026 GMT\n  hsts: false\n- host: api.harvardartmuseums.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:45:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: library.harvard.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:07:23 2026 GMT\n  hsts: false\ndomains:\n- domain: harvard.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: harvardartmuseums.org\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harvard/refs/heads/main/security/harvard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Libraries
- Museums
- Open Metadata
- OAI-PMH
---
