---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@conduitmail.app"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: conduitmail.app
  spf: true
hosts:
- cert_expires: Jan  4 02:25:37 2027 GMT
  host: conduitmail.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Conduit Mail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conduit Mail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Conduit Mail
provider_slug: conduitmail-app
slug: conduitmail-app-domain-security
source_filename: conduitmail-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conduitmail.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 02:25:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: conduitmail.app\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@conduitmail.app\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/conduitmail-app/security/conduitmail-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email
- Email Client
- Artificial Intelligence
- MCP
- AI Agents
- Productivity
- Automation
---
