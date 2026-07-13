---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "quovadisglobal.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:dns-manager@abdn.ac.uk"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: abdn.ac.uk
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.abdn.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  5 10:40:20 2026 GMT
  host: aura.abdn.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Aberdeen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Aberdeen, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Aberdeen
provider_slug: university-of-aberdeen
slug: university-of-aberdeen-domain-security
source_filename: university-of-aberdeen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abdn.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: aura.abdn.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 10:40:20 2026 GMT\n  hsts: false\ndomains:\n- domain: abdn.ac.uk\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:dns-manager@abdn.ac.uk\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-aberdeen/refs/heads/main/security/university-of-aberdeen-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Institutional Repository
- DSpace
- OAI-PMH
- United Kingdom
- Scotland
---
