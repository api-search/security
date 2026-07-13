---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:sysadmins@37signals.com"
  - 0 issue "amazon.com"
  dmarc: false
  dnssec: false
  domain: kamal-deploy.org
  spf: false
hosts:
- cert_expires: Aug 20 12:23:34 2026 GMT
  host: kamal-deploy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kamal Deploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kamal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kamal
provider_slug: kamal-deploy
slug: kamal-deploy-domain-security
source_filename: kamal-deploy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kamal-deploy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 12:23:34 2026 GMT\n  hsts: false\ndomains:\n- domain: kamal-deploy.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:sysadmins@37signals.com\"\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kamal-deploy/refs/heads/main/security/kamal-deploy-domain-security.yml
summary_line: TLSv1.3
tags:
- Deployment
- DevOps
- Docker
- Containers
- Zero Downtime
- Rolling Deploys
- Rails
- Ruby
- Open Source
- 37signals
- Basecamp
- On Premises
- Infrastructure
- CLI
- SSH
---
