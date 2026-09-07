---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: accuknox.com
  spf: true
hosts:
- cert_expires: Oct  4 07:18:38 2026 GMT
  host: accuknox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: help.accuknox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 17:17:11 2026 GMT
  host: cspm.accuknox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Accuknox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AccuKnox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AccuKnox
provider_slug: accuknox
slug: accuknox-domain-security
source_filename: accuknox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accuknox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:18:38 2026 GMT\n  hsts: false\n- host: help.accuknox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\n- host: cspm.accuknox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 17:17:11 2026 GMT\n  hsts: null\ndomains:\n- domain: accuknox.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accuknox/refs/heads/main/security/accuknox-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Cloud Security
- Cloud Native Application Protection Platform
- Kubernetes Security
- Runtime Security
- Zero Trust
- DevSecOps
- Compliance
- AI Security
- Vulnerability Management
- Container Security
---
