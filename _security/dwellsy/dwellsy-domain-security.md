---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dwellsy.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: dwellsy.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dwellsy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dwellsy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Dwellsy
provider_slug: dwellsy
slug: dwellsy-domain-security
source_filename: dwellsy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dwellsy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dwellsy.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dwellsy/security/dwellsy-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
---
