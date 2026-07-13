---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:abuse@tudelft.nl"
  - 0 issuewild "harica.gr"
  - 0 issuemail "harica.gr"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tudelft.nl
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: 4tu.nl
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: www.tudelft.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 22:09:22 2026 GMT
  host: djehuty.4tu.nl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 08:20:16 2026 GMT
  host: data.4tu.nl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tu Delft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delft University of Technology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Delft University of Technology
provider_slug: tu-delft
slug: tu-delft-domain-security
source_filename: tu-delft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tudelft.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: djehuty.4tu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 22:09:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: data.4tu.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:20:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tudelft.nl\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:abuse@tudelft.nl\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issuemail \"harica.gr\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: 4tu.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-delft/refs/heads/main/security/tu-delft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Library
- Open Data
- Netherlands
- Europe
---
