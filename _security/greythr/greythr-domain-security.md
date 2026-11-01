---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "rapidssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: greythr.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.greythr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Greythr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for greytHR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: greytHR
provider_slug: greythr
slug: greythr-domain-security
source_filename: greythr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greythr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: greythr.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"rapidssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/greythr/security/greythr-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- HR
- Payroll
- AI
- SaaS
---
