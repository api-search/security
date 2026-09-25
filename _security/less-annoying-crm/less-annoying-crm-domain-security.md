---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops@lessannoyingcrm.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lessannoyingcrm.com
  spf: true
hosts:
- cert_expires: Dec 13 07:31:32 2026 GMT
  host: lessannoyingcrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Less Annoying Crm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Less Annoying CRM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Less Annoying CRM
provider_slug: less-annoying-crm
slug: less-annoying-crm-domain-security
source_filename: less-annoying-crm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lessannoyingcrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 07:31:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lessannoyingcrm.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@lessannoyingcrm.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/less-annoying-crm/refs/heads/main/security/less-annoying-crm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Small Business
- Contact Management
- Software-as-a-Service
---
