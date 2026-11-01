---
description: ''
domains:
- caa:
  - 0 iodef "mailto:abuse@tudelft.nl"
  - 0 issuewild "harica.gr"
  - 0 issuemail "harica.gr"
  - 0 issue "harica.gr"
  - 0 issue "www.digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tudelft.nl
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.tudelft.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Delft University Of Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delft University of Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Delft University of Technology
provider_slug: delft-university-of-technology
slug: delft-university-of-technology-domain-security
source_filename: delft-university-of-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tudelft.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tudelft.nl\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:abuse@tudelft.nl\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issuemail \"harica.gr\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/delft-university-of-technology/security/delft-university-of-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Research
- Engineering
- Netherlands
- University
---
