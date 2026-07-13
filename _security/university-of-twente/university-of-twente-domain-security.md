---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "harica.gr"
  - 0 issuemail "harica.gr"
  - 0 iodef "mailto:scs-ra@utwente.nl"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: utwente.nl
  spf: true
hosts:
- cert_expires: Jan  8 10:17:33 2027 GMT
  host: www.utwente.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Twente Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Twente, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: University of Twente
provider_slug: university-of-twente
slug: university-of-twente-domain-security
source_filename: university-of-twente-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.utwente.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 10:17:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: utwente.nl\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"harica.gr\"\n  - 0 issuemail \"harica.gr\"\n  - 0 iodef \"mailto:scs-ra@utwente.nl\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-twente/refs/heads/main/security/university-of-twente-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Netherlands
- Open Science
---
