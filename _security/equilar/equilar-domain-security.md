---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:admininfo@equilar.com"
  - 0 issuewild "godaddy.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: equilar.com
  spf: true
hosts:
- cert_expires: Mar  2 20:56:41 2027 GMT
  host: www.equilar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Equilar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equilar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Equilar
provider_slug: equilar
slug: equilar-domain-security
source_filename: equilar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.equilar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 20:56:41 2027 GMT\n  hsts: null\ndomains:\n- domain: equilar.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:admininfo@equilar.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/equilar/security/equilar-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Human Resources
- Compensation
- Governance
- Data Analytics
---
