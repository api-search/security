---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: persistent.com
  spf: true
hosts:
- cert_expires: Feb 21 08:47:17 2027 GMT
  host: persistent.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Persistent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Persistent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Persistent
provider_slug: persistent
slug: persistent-domain-security
source_filename: persistent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: persistent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 08:47:17 2027 GMT\n  hsts: false\ndomains:\n- domain: persistent.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persistent/refs/heads/main/security/persistent-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Digital Engineering
- Enterprise Modernization
- IT Services
- Consulting
- Cloud
- Artificial Intelligence
- Software Product Engineering
---
