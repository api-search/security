---
description: ''
domains:
- caa:
  - 0 iodef "mailto:information.security@jisc.ac.uk"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "ssl.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jisc.ac.uk
  spf: true
hosts:
- cert_expires: Mar 26 10:27:11 2027 GMT
  host: www.jisc.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jisc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jisc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jisc
provider_slug: jisc
slug: jisc-domain-security
source_filename: jisc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jisc.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 26 10:27:11 2027 GMT\n  hsts: null\ndomains:\n- domain: jisc.ac.uk\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:information.security@jisc.ac.uk\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jisc/refs/heads/main/security/jisc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Technology
- Digital Services
- Research
- UK
---
