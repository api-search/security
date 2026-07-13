---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:it@khanacademy.org"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: khanacademy.org
  spf: true
hosts:
- cert_expires: Nov 11 17:18:53 2026 GMT
  host: www.khanacademy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Khan Academy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Khan Academy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Khan Academy
provider_slug: khan-academy
slug: khan-academy-domain-security
source_filename: khan-academy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.khanacademy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 17:18:53 2026 GMT\n  hsts: false\ndomains:\n- domain: khanacademy.org\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:it@khanacademy.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/khan-academy/refs/heads/main/security/khan-academy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- EdTech
- Online Learning
- Non-Profit
- K-12
---
