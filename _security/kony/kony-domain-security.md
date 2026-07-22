---
description: ''
domains:
- caa:
  - 128 issue "godaddy.com"
  - 128 iodef "mailto:CloudAdmin@temenos.com"
  - 128 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kony.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.kony.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kony, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kony
provider_slug: kony
slug: kony-domain-security
source_filename: kony-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kony.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: kony.com\n  dnssec: false\n  caa:\n  - 128 issue \"godaddy.com\"\n  - 128 iodef \"mailto:CloudAdmin@temenos.com\"\n  - 128 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kony/refs/heads/main/security/kony-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Low-Code
- Mobile
- Application Development
- Digital Banking
- Enterprise
- Acquired
---
