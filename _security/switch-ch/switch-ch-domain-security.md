---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "digicert.com; account=88646c566474fb435c2a73b7e885f93cee64611d831bca6d567ff2f5f8de6d76"
  - 0 issue "digicert.com; account=88646c566474fb435c2a73b7e885f93cee64611d831bca6d567ff2f5f8de6d76"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: switch.ch
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.switch.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Switch Ch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SWITCH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SWITCH
provider_slug: switch-ch
slug: switch-ch-domain-security
source_filename: switch-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.switch.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: switch.ch\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com; account=88646c566474fb435c2a73b7e885f93cee64611d831bca6d567ff2f5f8de6d76\"\n  - 0 issue \"digicert.com; account=88646c566474fb435c2a73b7e885f93cee64611d831bca6d567ff2f5f8de6d76\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/switch-ch/refs/heads/main/security/switch-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Education
- Infrastructure
- Open Source
- Security
---
