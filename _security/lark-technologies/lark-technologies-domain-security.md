---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@lark.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lark.com
  spf: true
hosts:
- cert_expires: Sep  8 16:19:14 2026 GMT
  host: www.lark.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:40:45 2026 GMT
  host: support.lark.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Zendesk-hosted help center
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: enroll.lark.com
  hsts: false
  https: true
  note: member enrollment application (enroll.production.lark.com)
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: larktechnologies.statuspage.io
  hsts: true
  hsts_max_age: 259200
  https: true
  note: Atlassian Statuspage; status.lark.com CNAMEs here but does not serve TLS
kind: domain-security
layout: security
method: probed
name: Lark Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lark, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lark
provider_slug: lark-technologies
slug: lark-technologies-domain-security
source_filename: lark-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 16:19:14 2026 GMT\n  hsts: false\n- host: support.lark.com\n  https: true\n  cert_expires: Sep 18 23:40:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Zendesk-hosted help center\n- host: enroll.lark.com\n  https: true\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\n  note: member enrollment application (enroll.production.lark.com)\n- host: larktechnologies.statuspage.io\n  https: true\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 259200\n  note: Atlassian Statuspage; status.lark.com CNAMEs here but does not serve TLS\nabsent_hosts:\n- api.lark.com\n- developer.lark.com\n- developers.lark.com\n- docs.lark.com\n- mcp.lark.com\n- trust.lark.com\n- dashboard.lark.com\n- partners.lark.com\nfindings:\n- id:\
  \ no-hsts-on-www\n  severity: low\n  detail: www.lark.com serves no Strict-Transport-Security header.\n- id: dmarc-not-reject\n  severity: low\n  detail: DMARC policy is p=quarantine rather than p=reject.\n- id: no-dnssec\n  severity: low\n  detail: lark.com is not DNSSEC-signed.\n- id: status-subdomain-tls-broken\n  severity: low\n  detail: >-\n    status.lark.com CNAMEs to larktechnologies.statuspage.io but the TLS handshake\n    fails (curl exit 000); the status page is only reachable at the statuspage.io\n    hostname.\n- id: caa-iodef-present\n  severity: info\n  detail: 'CAA iodef points at mailto:security@lark.com — matches the published disclosure contact.'\ndomains:\n- domain: lark.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@lark.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lark-technologies/refs/heads/main/security/lark-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Chronic Disease Management
- Diabetes
- Hypertension
- Weight Management
- Artificial Intelligence
- Health Coaching
- Remote Patient Monitoring
- Telehealth
---
